# Simpsons Characters Identification

This repository contains code for identifying Simpsons characters using a neural network model. The dataset used for training and testing the model is sourced from Kaggle's ["The Simpsons Characters Dataset"](https://www.kaggle.com/datasets/alexattia/the-simpsons-characters-dataset).

## Dataset
The dataset consists of images of various Simpsons characters, each labeled with the corresponding character's name. It encompasses a wide range of characters from the Simpsons universe.

## Neural Network Model
The identification task is approached using a neural network model implemented with PyTorch. The model architecture follows a sequential approach and includes convolutional layers, max-pooling layers, dropout layers, and fully connected layers for classification.

The sequential neural network architecture is structured as follows:
- **Convolutional Layers**: The model starts with a convolutional layer (`nn.Conv2d`) followed by a rectified linear unit (ReLU) activation function (`nn.ReLU`). Max-pooling layers (`nn.MaxPool2d`) are used to downsample the feature maps.
- **Dropout**: Dropout layers (`nn.Dropout`) are introduced to prevent overfitting by randomly setting a fraction of input units to zero during training.
- **Flatten**: After the convolutional layers, the output is flattened using `nn.Flatten()` to prepare for the fully connected layers.
- **Fully Connected Layers**: The flattened output is passed through one or more fully connected layers (`nn.Linear`) with ReLU activation functions.

## Performance
After training the model on the dataset, it achieved an accuracy of approximately 56% on the test set. While this accuracy may not be exceptionally high, it demonstrates the model's capability to recognize Simpsons characters to a certain extent. Further enhancements to the model architecture, data preprocessing, and training strategy could potentially improve its performance.

## Acknowledgments
- The dataset used in this project is sourced from Kaggle, specifically from [The Simpsons Characters Dataset](https://www.kaggle.com/datasets/alexattia/the-simpsons-characters-dataset).
- Inspiration and guidance for building the neural network model were drawn from various online tutorials and resources.
