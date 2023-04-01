# Gesture-Recognition-using-the-3D-CNN-and-CNN-RNN
>
> This project is made to recognize the hand gestures using the CNN(Convolutional Neural Network) which is then can be used for automation of the home appliances.

## Table of Contents

## General Information

### Problem Statement

The problem statement is to recognize the hand gestures using the CNN(Convolutional Neural Network).The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:

- Thumbs up:  Increase the volume
- Thumbs down: Decrease the volume
- Left swipe: 'Jump' backwards 10 seconds
- Right swipe: 'Jump' forward 10 seconds  
- Stop: Pause the movie

## Dataset

The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use.
The data is in a zip file. The zip file contains a 'train' and a 'val' folder with two CSV files for the two folders. These folders are in turn divided into subfolders where each subfolder represents a video of a particular gesture. Each subfolder, i.e. a video, contains 30 frames (or images). Note that all images in a particular video subfolder have the same dimensions but different videos may have different dimensions. Specifically, videos have two types of dimensions - either 360x360 or 120x160 (depending on the webcam used to record the videos).
Each row of the CSV file represents one video and contains three main pieces of information - the name of the subfolder containing the 30 images of the video, the name of the gesture and the numeric label (between 0-4) of the video.

## Neural Network Used

### 3D Convolutional Neural Network

A 3D Convolutional Neural Network (CNN) is a deep learning algorithm that uses 3D convolutions to extract features from spatio-temporal data, such as videos or medical imaging. It can capture both spatial and temporal dependencies in the data, making it useful for tasks such as action recognition or disease diagnosis.

### Convolutional Neural Network - Recurrent Neural Network

A CNN-RNN model is a type of neural network architecture that combines Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs) to process sequential data such as speech, text, or time series data. The CNNs can extract local features from the input data, while RNNs can capture long-term dependencies and temporal dynamics. The output of the CNNs is fed into the RNNs to generate predictions based on the learned representations. This model has been used for tasks such as speech recognition, language translation, and video analysis.

## Results

We have achieved an accuracy of 98% on the test data.

## Contact

Created by [@sukhijapiyush] - feel free to contact me!

## License

This project is open source and available under the [GNU General Public License v3.0].
