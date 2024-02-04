# Self-Driving-Car
The CNN model is made for automonous driving of car, first we have given the model the images of driving a car in manual mode to learn from it and extract proper features from it.
While driving the car we have given the images of center, right, and left side of the dashboard to properly analyze how to drive the car.
<br><br>
We first balanced the data so that so data do not repeat as the model will learn that pattern only so we needed to balance it. We then applied the data preprocessing like split the data in train and test data.
We have also augmented the data like zooming the image, flipping it, blurring it so that our model trains well and get various type of data.
<br>
## Neural Network Architecture
We have created 4 convolutional layer with different filter sizes such as (24, 36, 48, 64). We also defined the striding so that our spatial dimension gets reduced. The activation function used is the Exponential Linear Unit (ELU). 
<br>
We then flatten the output coming from convolutional layer to 1D array to feed them into the fully connected network. We have 3 fully connected hidden layer with different number of neuron in each layer. The final output layer has only 1 neuron which gives the probability of the stearing angle. The mean squared error (MSE) cost function used for training model.
<br><br>
drive.py file connects the udacity simulator and our model the simulator sends the snapshot of the dashboard of the car that is preprocessed and then given to the model which predicts the steering angle that is given back to car in simulator.

# Video Demonstation
<a href="https://drive.google.com/file/d/1LdziNWauoXAnktX89WnX0spevTBp9wuv/view?usp=sharing">Video Link</a>
# Simulation setup
Install the Unity Hub which is needed to run the udacity simulation 
https://unity.com/download
<br><br>
Now install the Udacity simulator from https://github.com/udacity/self-driving-car-sim
based on your computer configuration download the version accordingly
<br><br>
# Installation of anaconda
Install and setup anaconda on your computer from the following link. <br>
https://www.anaconda.com/download
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
## Install all these python packages
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
## Now run the following command
```
python drive.py
```

<br><br>
Now open the simulator in Autonomous mode 

