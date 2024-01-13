# Self-Driving-Car
The CNN model is made for automonous driving of car, first we have given the model the images of driving a car in manual mode to learn from it and extract proper features from it.
While driving the car we have given the images of center, right, and left side of the dashboard to properly analyze how to drive the car.
<br>
We first balanced the data so that so data do not repeat as the model will learn that pattern only so we needed to balance it. We then applied the data preprocessing like split the data in train and test data.
We have also augmented the data like zooming the image, flipping it, blurring it so that our model trains well and get various type of data.
<br>
# Network Architecture
Four convolutional layers with increasing filter sizes (24, 36, 48, 64).
The first three layers have a stride of (2, 2), which reduces spatial dimensions.
# Video Demonstation
Video Link : https://drive.google.com/file/d/1LdziNWauoXAnktX89WnX0spevTBp9wuv/view?usp=sharing
# Simulation setup
Install the Unity Hub which is needed to run the udacity simulation 
https://unity.com/download
<br><br>
Now install the Udacity simulator from https://github.com/udacity/self-driving-car-sim
based on your computer configuration download the version accordingly
<br><br>
Now create an separate enviroment for self driving car
```
conda create -n sdcar python=3.7 -y
```
Now activate this environment
```
conda activate sdcar
```
<br><br>
# Install all these python packages
<br>
opencv-contrib-python
<br>
numpy
<br>
matplotlib
<br>
tensorflow
<br>
keras
<br>
python-socketio==4.6.1
<br>
Flask
<br>
eventlet
<br>
python-engineio==3.13.2
<br>

<br><br>
# Now run the following command
```
python drive.py
```

<br><br>
Now open the simulator in Autonomous mode 

