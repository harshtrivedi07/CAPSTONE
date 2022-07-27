# CAPSTONE-PROJECT
# Development of ML models to predict client emotions based on facial expressions and audio input in various online meeting platforms.

# Introduction
The aim of this project is to build a machine learning model which can predict the emotions of a person based on the facial expression and speech of that person and then deploying this model on the webpage of CogniXR health. CogniXR health is start-up which provides telehealth services. In this project we have build 2 separate models which can predict the emotion of the person. One model will used to predict the emotions from the image while the other one will be used to predict the emotion from the speech of the person.  

# Models used for predicting emotion from facial expressions
- Used VGG16 with imagenet weights
- Accuracy : 76.43%
- Precision : 52.73%
- Recall : 40.98%
- AUC : 67.83%

# Models used for predicting emotion from audio input
- Used CNN model
- Accuracy : 84.83%
- Precision : 82.14%
- Recall : 81.86%
- AUC : 84.90%

# API implementation (Model_API.py)
- Used flask for making API
- Loaded the save models in the API and performed predictions.
- Passed the predicted values from the API to the webpage to display the results according.
- Webpage displays two bar charts and the predictions of the video and audio predictions made by the API.

# How to run the project
- Running the Model_API.py will load all the models and run all the functions.
- After successfully running the Model_API.py file, index.html will be loaded on the localhost.
- Once we open the localhost link, we will be asked to upload the video, once we upload the video, the video will be send to the API for predicting its output.
- Once the API has predicted the video input and the audio input the data will be passed to the HTML page and the results willbe displayed in the form of Bar charts and image slider.
