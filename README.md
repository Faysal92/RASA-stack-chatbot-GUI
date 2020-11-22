# Chatbot-with-Rasa-stack (core + nlu)
HR Chatbot with Rasa (core + nlu)

You should have Python3.6 and pip manager installed on your machine.

Outline : 

First of all, we need to create anaconda environment (to not have a conflict between packages for smooth installation) using the python version 3.6 as an interpreter through the following command : 

conda create -n yourenvname python=3.6 anaconda  

then activate it, using : activate yourenvname 

 
Instaltion : The following modules are required : 
                 rasa_core==0.14.0 
                 rasa_sdk 
                 rasa_core_sdk 
                 rasa_nlu[spacy] 
                 nltk 
                 numpy 
                 pandas 
                 scikit-learn 
                 flask 
                 Gunicorn 

These modules are in requirements.txt file, we can install them in one command using : pip install –r requirements 

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
