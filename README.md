
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
 
 Corresponding notebook for CNN(Convolutional Neural Networks)Model building: https://github.com/shaanusyed/CNN-MODEL/blob/e5594d0d7c47318b8cd3c2e4ce75f4dbe16d24e9/CATS%20and%20DOGS%20CNN%20Model.ipynb

 
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

<img width="457" alt="image" src="https://github.com/user-attachments/assets/a4d0c4d4-156c-40be-ae48-ddce0559273f" />

#### Loss graph plot:

<img width="458" alt="image" src="https://github.com/user-attachments/assets/88ef7af5-dce5-42d0-b321-8c8e8c183bea" />

### Step 6: Before applying regularization the accuracy
Accuracy : 84%
Validation accuracy : 82%
(for 5 epochs of validation data below are the accuracy percentages) 
Epoch 1: Validation Accuracy = 70.91%
Epoch 2: Validation Accuracy = 79.09%
Epoch 3: Validation Accuracy = 77.70%
Epoch 4: Validation Accuracy = 82.26%
Epoch 5: Validation Accuracy = 82.87%

## Step 7: Tested with sample images data
. Getting sometimes wrong predictions
. So went for regularization in the next step

### Step 8: Applying BacthNormalization and Dropout techniques to predict better
Again built the model with BatchNormalization and Dropout technique

### STEP 9 - Performance Analysis: model accuracy is plotted and after applying regularization
Training and validation accuracy across 5 epochs, plotted the accuracy and loss graphs

#### Accuracy graph:

<img width="457" alt="image" src="https://github.com/user-attachments/assets/1bbaa474-8913-4f3c-8963-e27223fc0d0e" />

#### Loss graph plot:

<img width="452" alt="image" src="https://github.com/user-attachments/assets/c6c5dbea-c7d0-4d90-bd83-3bbebe267b36" />

## Fianl accuracy after regularization:
Train Accuracy = 89%
Got validation accuracy as 77%

(for 5 epochs of validation data below are the accuracy percentages) 
Epoch 1: Validation Accuracy = 60.30%
Epoch 2: Validation Accuracy = 73.65%
Epoch 3: Validation Accuracy = 79.83%
Epoch 4: Validation Accuracy = 78.57%
Epoch 5: Validation Accuracy = 71.26%

### Step 10: Tested the model on the sample data images

## Conclusion : 
Model is able to giving correct predictions except some images before and after regularization.
We can stick to basic model as difference between train and validation accuracy is smaller than regularization technique applied accuracy difference.


<img width="266" alt="image" src="https://github.com/user-attachments/assets/0f049bc0-02f0-41cb-98c3-396c7842aeaf" />

<img width="323" alt="image" src="https://github.com/user-attachments/assets/1e3e7825-54b3-48bf-8d7a-06c62eafcfc9" />


