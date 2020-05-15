# HackerEarth-Deep-Learning-Challenge

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
