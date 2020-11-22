# HR-Recruiter-Chatbot-with-Rasa
HR Recruiter Chatbot with Rasa

You should have Python3.6 and pip manager installed on your machine.

Here is how to install the dependencies

pip install -r requirements.txt



And then train the Dialogue model by,

1- And then train the NLU model by running, train nlu by running : python nlu_training.py
   this will create a NLU model under models directory.

2- train rasa core by typing :
   python -m rasa_core.train -d domain.yml -s data/stories.md -o models/dialogue -c policy.yml


3- Run Bot server using : 
   python -m rasa_core.run --enable_api -d models/dialogue -u models/nlu/default/current --cors "*" -o out.log --endpoints endpoints.yml --port 5800 --credentials credentials.yml


4- Run web app by (or just open index.html)
   running web_app.py


5- python -m rasa_core_sdk.endpoint --actions action









You can ; - Start a new terminal and type the command,
          - python train_dialogue.py
          - And dynamically create storyboard and training data for your bot.
