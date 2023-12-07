# Chatbot Deployment with Flask and JavaScript

In this tutorial we deploy the chatbot I created in [this](https://github.com/Pranjal0310/Neural-Chatbot) tutorial with Flask and JavaScript.


Serve only the Flask prediction API. The used html and javascript files can be included in any Frontend application (with only a slight modification) and can run completely separate from the Flask App then.

## Initial Setup:
This repo currently contains the starter files.

Clone repo and create a virtual environment
```
$ git clone https://github.com/Pranjal0310/Neural-Chatbot.git
$ cd Neural-Chatbot
$ pip install virtualenv
$ virtualenv env
$  .\env\Scripts\activate.ps1
```
Install dependencies
```
$ (venv)pip install Flask torch torchvision nltk
```
Install nltk package
```
$ (venv) python
>>> import nltk
>>> nltk.download('punkt')
```
Modify `intents.json` with different intents and responses for your Chatbot

Run
```
$ (venv) python train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
$ (venv) python chat.py
```
For Running the chatbot in the server 
```
$ (venv) python app.py
```
