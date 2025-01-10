
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

 Corresponding notebook for Data Loading:  https://github.com/shaanusyed/CNN-MODEL/blob/main/Cats%20and%20Dogs%20DATA%20Preprocessing.ipynb
 
 Corresponding notebook for Data Loading:  https://github.com/shaanusyed/CNN-MODEL/blob/main/CATS%20and%20DOGS%20CNN%20Model%20using%20Keras.ipynb

### STEP 1 - Initialization: importing necessary libraries and modules.

### STEP 2 - Loading Dataset: loading the dataset from os module and checking its details.
1.Tranforamtion: resizing image shape
2.Saving data into pickle file
3.Loading data from pickle file

### STEP 3 - Building CNN Sequential Model: CNN model consists of the following Sequential layers:
Input layer.
Three convolutional layers with ReLU activation function and with same number of filters.
Three max pooling layers following the convolutional layers.
Flattening layer.
One dense/fully connected layer with ReLU activation function.
Output layer with 'Sigmoid' activation function.


### STEP 4 - Model Training: model is compiled and trained using the following configurations:
Optimizer: Adam.
Loss function: binary_crossentropy.
Epochs: 5
batch size = 64
metrics: accuracy
validation data = 10% of whole data

### STEP 5 - Performance Analysis: model accuracy is plotted and analyzed across the 5 epochs.
Training and validation accuracy across 5 epochs, plotted the accuracy and loss graphs

#### Accuracy graph
<img width="421" alt="image" src="https://github.com/user-attachments/assets/e333a84b-7f6a-47b1-8303-e92380d9ec5d" />

#### Loss graph plot:
<img width="422" alt="image" src="https://github.com/user-attachments/assets/8c646c8c-4c7f-47a9-b829-f94b4d4b5ed4" />


### Step 6: Before applying regularization the accuracy
Accuracy : 96%
Validation accuracy : 85%

## Step 7: Tested with sample images data
. Getting sometimes wrong predictions
. So went for regularization in the next step

### Step 8: Applying BacthNormalization and Dropout techniques to predict better
Again built the model with BatchNormalization and Dropout technique

### STEP 9 - Performance Analysis: model accuracy is plotted and after applying regularization
Training and validation accuracy across 5 epochs, plotted the accuracy and loss graphs

#### Accuracy graph
<img width="410" alt="image" src="https://github.com/user-attachments/assets/e32d074a-bc7a-4b5e-862f-b5377edd971c" />

#### Loss graph plot:
<img width="410" alt="image" src="https://github.com/user-attachments/assets/3aac3f51-c46f-4368-a7cc-faa03eadcf91" />


## Fianl accuracy after regularization:
Got validation accuracy as 77.96%

(for 5 epochs of validation data below are the accuracy percentages) 
Epoch 1: Validation Accuracy = 50.96%
Epoch 2: Validation Accuracy = 74.09%
Epoch 3: Validation Accuracy = 64.48%
Epoch 4: Validation Accuracy = 76.48%
Epoch 5: Validation Accuracy = 77.96%

### Step 10: Tested the model on the sample data images

## Conclusion : Model is able giving correct predictions

<img width="266" alt="image" src="https://github.com/user-attachments/assets/0f049bc0-02f0-41cb-98c3-396c7842aeaf" />
