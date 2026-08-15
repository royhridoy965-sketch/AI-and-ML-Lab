# CNN Image Classification - Rock Paper Scissors

## Project Overview

This project implements a Convolutional Neural Network (CNN) for classifying hand gesture images into three classes:

- Rock
- Paper
- Scissors

The project was developed using Python and PyTorch in Google Colab.

## Dataset

The Rock Paper Scissors dataset contains three classes:

- Rock
- Paper
- Scissors

The dataset was downloaded programmatically in Google Colab.

## Image Preprocessing

The following preprocessing techniques were applied using `torchvision.transforms`:

- Resize images to 128 × 128
- Convert images to tensors using `ToTensor()`
- Normalize images using mean and standard deviation

## Data Split

The dataset was divided into:

- 80% Training data
- 20% Validation data

Batch size: 64

## CNN Architecture

The CNN model contains:

- 3 Convolutional layers
- ReLU activation functions
- Max Pooling layers
- Fully Connected layers
- 3 output classes

The model was trained using:

- Loss Function: CrossEntropyLoss
- Optimizer: Adam
- Learning Rate: 0.001
- Epochs: 10

## Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

Training and validation loss and accuracy graphs were also generated.

## Model File

The trained model is saved as:

`model/CNN_RPS.pth`

## Notebook

The complete implementation is available in:

`CNN_RPS.ipynb`

## Tools and Technologies

- Python
- PyTorch
- Torchvision
- Scikit-learn
- Matplotlib
- Google Colab
- GitHub
