# Potato-disease-Classification-using-CNN

## Overview
This project uses Convolutional Neural Networks (CNNs) implemented with TensorFlow and Keras to classify potato disease images. The dataset is organized into classes representing different diseases.

## Dataset
The dataset (https://www.kaggle.com/datasets/arjuntejaswi/plant-village ) is a set of potato disease images basically potato_early_blight, potato_late_blight, potato_healthy and is extracted using TensorFlow's `image_dataset_from_directory` function. It consists of images with a size of 256x256 pixels, grouped into batches of 32, and having 3 color channels.

## Data Preparation
Images are preprocessed using resizing and rescaling operations. Additionally, data augmentation is performed to enhance the training set.

## Model Architecture
The CNN model is defined using TensorFlow's Sequential API. It consists of convolutional layers, max-pooling layers, and fully connected layers. The output layer uses softmax activation for multi-class classification.

## Training
The dataset is split into training (80%), validation (10%), and test (10%) sets. The model is trained for 50 epochs using the Adam optimizer and Sparse Categorical Crossentropy loss.

## Model Evaluation
The model is evaluated on the test set, and accuracy scores are displayed.

## Visualization
Training and validation accuracy/loss curves are plotted to visualize the model's performance.

## Prediction
A function of the model is created which accepts the image as the input and is used to predict the class of a sample image from the test set, and predictions for a set of 9 images are displayed along with actual classes and confidence levels.
