# Image Detection - Computer Vision

# About This Project
This project was implemented for final project submission for Buan 6V99 - Special Topics in Business Analytics - Deep Learning by myself, Varun Banda and Swetha ponugoti.<br/>
This was one of two submissions for an inclass Kaggle competition and finished in 1st place.<br/>
Kaggle Competition: https://www.kaggle.com/c/final-project-dl-spring-2020/leaderboard

# Objective:
The object of this project is to accurately predict the type of dog breed from any given image.<br/>
This type of classification is a common problem in computer vision and has user applications in tools like Google Lens.<br/>
Dog Breed classification is an enhanced classification problem than regular object detection since prediction granularity has increased from dogs vs objects to different types of dogs. 

# Data : ImageWoof
Imagewoof is a subset of 10 classes of dogs from Imagenet. These images are not that easy to classify, since they're all dog breeds. The breeds are: Australian terrier, Border terrier, Samoyed, Beagle, Shih-Tzu, English foxhound, Rhodesian ridgeback, Dingo, Golden retriever, Old English sheepdog.<br/>
The Data set has been taken from: https://github.com/fastai/imagenette

# Data Transformations: 

The images have been resized to 299x299<br/>
Random rotation of 25 degrees was applied<br/>
Horizontal flip with p=0.5<br/>
Vertical flip with p=0.5<br/>
Normalized the RGB values

# Model: 
PreTrained ResNext Model<br/>
Learning Rate = 0.0001<br/>
Optimization Function = Adam<br/>
Learning Rate Scheduler = StepLR

# Accuracy: 
Train Accuracy: 81.81<br/>
Validation Accuracy: 95.6<br/>
Kaggle Test Accuracy: 94.8
