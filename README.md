# Bird Classification using VGG16 Transfer Learning

## About the Project

This project demonstrates the use of transfer learning with the VGG16 model for classifying bird images into 525 different classes. The dataset used in this project consists of bird images categorized into training, testing, and validation sets. The goal of this project is to build a model that can accurately classify bird images into their respective classes.

## Dataset

The dataset used in this project is the "100 Bird Species" dataset available on Kaggle. You can download the dataset from the following link:

[525 Bird Species Dataset](https://www.kaggle.com/datasets/gpiosenka/100-bird-species)

## Code Explanation

- **Model Creation**: The VGG16 model is used as the base model for transfer learning. The top layer of the VGG16 model is removed, and a custom fully connected layer is added as the output layer with softmax activation function for multi-class classification.

- **Data Preparation**: The dataset is organized into training, testing, and validation directories. ImageDataGenerator is used for data augmentation and preprocessing.

- **Model Training**: The model is compiled with categorical crossentropy loss and Adam optimizer. It is trained on the training set and evaluated on the validation set for 8 epochs.

- **Model Evaluation**: The model's performance is evaluated using the validation set, achieving an accuracy of approximately 73.49%.

- **Model Saving and Testing**: The trained model is saved as `model/BirdClassification.h5` and can be used for making predictions on new bird images. A function is defined to load the model and predict the class of a given image.

## Files

- `birdClassification.ipynb`: Jupyter notebook containing the code for model creation, training, evaluation, and testing.
- `dataset.txt`: Text file containing the link to the dataset used in the project.
- `model/BirdClassification.h5`: Saved model file containing the trained bird classification model.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/praiseprince/birdClassification.git
