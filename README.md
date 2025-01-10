
# Convolutional Neural Networks - Image Classification

The objective of this project is to carry out supervised image classification on a collection of cats and dogs images. It employs a convolutional neural network design and applies sigmoid activation function and transformations to recognize the category of images from a predefined set of 2 classes (Cats and Dogs)


## Data Set

From Kaggle : https://www.kaggle.com/datasets/arpitjain007/dog-vs-cat-fastai
The dataset has the following features:

Consists of 23,500 color images in 2 classes, with 11,500 mages per each class.
Classes: Cats, Dogs

Test sample data set : https://drive.google.com/drive/u/0/folders/1dZvL1gi5QLwOGrfdn9XEsi4EnXx535bD
The dataset has the following features: 

Used For: To test our model after model fitted
Consists of 400 images of both classes of Cats and Dogs
Classes: Cats, Dogs

## Classification: Keras Tensorflow 
### Corresponding notebook for Data Loading: Cats and Dogs DATA Preprocessing.ipynb
### Corresponding notebook for Data Loading: CATS and DOGS CNN Model using Keras.ipynb

### STEP 1 - Initialization: importing necessary libraries and modules.

### STEP 2 - Loading Dataset: loading the dataset from keras library and checking its details.

### STEP 3 - - Building CNN Model: CNN model consists of the following Sequential layers:

Input layer.
Three convolutional layers with ReLU activation function and with same number of filters.
Three max pooling layers following the convolutional layers.
Flattening layer.
One dense/fully connected layers with ReLU activation function.
Output layer with 'Sigmoid' activation function.


### STEP 4 - Model Training: model is compiled and trained using the following configurations:

Optimizer: Adam.
Loss function: binary_crossentropy.
Batch size: 64
Epochs: 5

### STEP 5 - Performance Analysis: model accuracy is plotted and analyzed across the epochs.

Training and validation accuracy across epochs (Tensorflow):

![Screenshot 2025-01-10 151025](https://github.com/user-attachments/assets/5c9c9b70-bb96-4649-a5b7-28754b93645d)























