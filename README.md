# HR-Chatbot-with-Rasa
HR Chatbot with Rasa

You should have Python3.6 and pip manager installed on your machine.

Here is how to install the dependencies

pip install -r requirements.txt



Let's create the Dialogue model ,

1- Train the NLU model by running : python nlu_training.py
   this will create a NLU model under models directory.

2- train rasa core by typing :
   python -m rasa_core.train -d domain.yml -s data/stories.md -o models/dialogue -c policy.yml


3- Run Bot server using : 
   python -m rasa_core.run --enable_api -d models/dialogue -u models/nlu/default/current --cors "*" -o out.log --endpoints endpoints.yml --port 5800 --credentials   credentials.yml


4- Run web app by (or just use index.html)
   running app.py


5- Custom Actions will be called by rasa open source assistant using : python -m rasa_core_sdk.endpoint --actions actions









You can ; - Start a new terminal and type the command,
          - python train_dialogue.py
          - And dynamically create storyboard and training data for your bot.
