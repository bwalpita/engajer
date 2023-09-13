colab notebook containe the real own model and steps (engager (1).ipynb)


this recomendation api developed with python fastapi


install this libraries
pip install fastapi,uvicorn
pip install requests

and the model is used for 'reberta base Model'
    but this model not implemented in this api script because we can't run the model local machine its require high ram, Cpu .

    so testing perpose we add dirrect hosted huggingface api for the Reberta base model , so in this test api 
    we can run and test local machine withoit any resources


how to run the api locally without any hardware resources?
    go to huggingface and cretae account to get api key its free , and video_recomend_api_QA_R_model.py containe this line youre need to put the api in here      headers = {"Authorization": f"Bearer {'api key'}"}  

    go to video_recomend_api_QA_R_model.py saved in folder and open 'CMD'
    after type uvicorn video_recomend_api_QA_R_model:app --reload
    this will show the url likes this http://127.0.0.1:8000 . copy to run on browser and change the url into http://127.0.0.1:8000/docs  
    it will show swagger api page and you can type the question and it will give related video link 
