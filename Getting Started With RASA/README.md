# The Starter (Default) Bot

The starter example is designed to help you see and run the out-of-the-box working chatbot.

## How to get the Starter example?

pip install rasa

python -W ignore -m rasa init --no-prompt

The rasa init command creates all the files that a Rasa project needs and trains a simple bot on some sample data. If you leave out the --no-prompt flag you will be asked some questions about how you want your project to be set up.


### What’s inside this example?

This example contains some training data and the main files needed to build an assistant on your local machine. The formbot consists of the following files:

    data/nlu.md contains training examples for the NLU model
    data/stories.md contains training stories for the Core model
    config.yml contains the model configuration
    domain.yml contains the domain of the assistant
       

### How to use this example?    

    Train a Rasa model containing the Rasa NLU and Rasa Core models by running:

    python -W ignore -m rasa train

    The model will be stored in the /models directory as a zipped file.

    In another window:

    python -W ignore -m rasa shell --quiet --cors * -m models 

    This will load the assistant in your command line for you to chat.
    

### Sample Chat   
```
Your input ->  Hi                                                                                                                                                                                           
Hey! How are you?
Your input ->  I am good and you?                                                                                                                                                                           
Great, carry on!
Your input ->  I am happy                                                                                                                                                                                   
Great, carry on!
Your input ->  I am sad                                                                                                                                                                                                                                                                                                                                                                             
Here is something to cheer you up:
Image: https://i.imgur.com/nGF1K8f.jpg
Did that help you?
Your input ->  are you bot?                                                                                                                                                                                
I am a bot, powered by Rasa.
Your input ->  okay, Thanks!                                                                                                                                                                                
Bye
Your input -> /stop
```                                                                                                                                                                                              

Reference

[https://rasa.com/docs/getting-started/]
