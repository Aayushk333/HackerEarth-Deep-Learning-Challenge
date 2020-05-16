# HackerEarth-Deep-Learning-Challenge

# Detect emotions of your favourite toons : Solution and Approach

## Context

This dataset is created for the Hackerearth Deep Learning Challenge of detection of emotions of cartoon characters from a video sample.

## Problem statement

The International Day of Happiness is celebrated globally on March 20 every year with an objective to promote happiness and well-being as a fundamental human right for all. On this International Day of Happiness, we are bringing back all the joy and happiness for you. This fun challenge requires you to build a model that detects emotions of your favorite characters of the iconic toon show—Tom and Jerry.

## Task

You are required to extract frames from a video clip that is provided in the dataset and classify the primary character’s emotion into one of the following five classes:

* Angry
* Happy
* Sad
* Surprised
* Unknown

### NOTE

1. The character prioritization is Tom > Jerry > Others.
2. In case a frame does not contain Tom or Jerry’s faces for emotion detection, it is classified as ‘Unknown’,

## Data

The dataset contains two video files and two .csv files. These files perform the following tasks:

* Train Tom and jerry.mp4: Video file used for training
* Train.csv: Contains human-generated labels for 298 frames [Framerate=5] from the training video
* Test Tom and jerry.mp4: Video file to detect emotions on the face
* Results.csv: Contains 186 frames [Framerate=5] from the test video in .csv format


### This model can be used for various purposes like :

* Screen time of a particular character 
* Screen time of a particular emotion 
* Character recognition

## Insights from the code 

1. The dataset for training has only 298 frames which are very less to train a model from scratch. Hence I have used data augmentation to increase the size of training dataset and hence to reduce overfitting to a large extent.
2. The actual predicted values of test images have not been provided and hence testing accuracy cannot be found out. In place of that I have used validation accuracy as a metric to evaluate my model’s performance.
3. It can be observed that VGG-16 performs better than the self proposed CNN architecture. The main reason for this is that out dataset is very small and hence cannot be used to train a Convolution Neural Network from scratch.
4. Overfitting is observed in case of both Self proposed architecture as well as VGG-16 pre- trained model.
5. The Proposed CNN architecture was able to achieve a validation accuracy of around 88% in case of proposed CNN and 94.3% in case of VGG-16 model.

