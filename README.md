# Gesture Recognition Project README

## Introduction
This project aims to develop a cool feature for smart TVs that can recognize five different gestures performed by the user, enabling users to control the TV without using a remote. The gestures include thumbs up, thumbs down, left swipe, right swipe, and stop, each corresponding to a specific command.

## Problem Statement
The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific action:

- Thumbs up: Increase the volume
- Thumbs down: Decrease the volume
- Left swipe: Jump backward 10 seconds
- Right swipe: Jump forward 10 seconds
- Stop: Pause the movie

## Dataset Overview
The training data consists of several hundred videos categorized into one of the five classes. Each video, typically 2-3 seconds long, is divided into a sequence of 30 frames (images). These videos were recorded by various people performing one of the five gestures in front of a webcam, similar to how the smart TV will be used.

The data is provided in a zip file, which contains 'train' and 'val' folders, each with two CSV files. These folders are further divided into subfolders, where each subfolder represents a video of a particular gesture. Each video subfolder contains 30 frames/images. Notably, all images in a particular video subfolder have the same dimensions, but different videos may have different dimensions (360x360 or 120x160).

Each row of the CSV file represents one video and contains three main pieces of information: the name of the subfolder containing the 30 images of the video, the name of the gesture, and the numeric label (between 0-4) of the video.

## Project Structure
1. **Data Preprocessing**: Preprocess the videos to standardize dimensions and format them for model input.
2. **Model Development**: Train a deep learning model on the training data to recognize gestures.
3. **Model Evaluation**: Evaluate the model's performance on the validation dataset.
4. **Inference**: Apply the trained model for gesture recognition on unseen data.

## Getting Started
To get started with the model building process, follow these steps:

1. **Download the Data**: Obtain the dataset provided in a zip file.
2. **Extract the Data**: Unzip the downloaded file to access the 'train' and 'val' folders containing the training and validation datasets, respectively.
3. **Preprocess the Data**: Preprocess the videos to standardize dimensions and format them for model input.
4. **Model Development**: Train a deep learning model using the preprocessed training data.
5. **Model Evaluation**: Evaluate the trained model's performance on the validation dataset.
6. **Inference**: Apply the trained model for gesture recognition on unseen data.

## Dependencies
Ensure you have the following dependencies installed:
- Python 3.x
- TensorFlow
- NumPy
- OpenCV
- Pandas
- Matplotlib

## Contributors
- Mayur Pardeshi
- Ashish Amber


