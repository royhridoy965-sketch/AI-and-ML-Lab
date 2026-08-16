# CNN Image Classification - Rock Paper Scissors

## Project Overview

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify Rock Paper Scissors hand gesture images into three classes:

- Rock
- Paper
- Scissors

The project was developed using Python, PyTorch and Google Colab.

## Dataset

The Rock Paper Scissors dataset contains three classes:

- Rock
- Paper
- Scissors

The dataset was downloaded programmatically using `torchvision.datasets.ImageFolder` from the GitHub repository.

## Image Preprocessing

The following preprocessing techniques were applied using `torchvision.transforms`:

- Resize images to 128 × 128
- Convert images to tensors using `ToTensor()`
- Normalize images using:

```text
Mean = [0.485, 0.456, 0.406]
Std  = [0.229, 0.224, 0.225]
## Data Split

The dataset contains 2520 images and was divided into three subsets:

- Training: 1764 images (70%)
- Validation: 378 images (15%)
- Test: 378 images (15%)

Batch size: 32

## CNN Architecture

The CNN model consists of:

- Convolutional layers using `nn.Conv2d`
- ReLU activation using `nn.ReLU()`
- Max Pooling using `nn.MaxPool2d`
- Fully Connected layers using `nn.Linear`
- Output layer with 3 classes

### Training Configuration

- Loss Function: `CrossEntropyLoss`
- Optimizer: `Adam`
- Epochs: 10

## Model Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Test Set Results

Test Accuracy: **100%**

All three classes achieved:

- Precision: 1.00
- Recall: 1.00
- F1-Score: 1.00

The test set contains 378 images.

## Custom Phone Image Testing

10 custom smartphone images were collected and stored in:

`CNN/dataset/`

The trained CNN was used to classify these real-world images.

For each image, the notebook displays:

- Actual Class
- Predicted Class
- Confidence Percentage

### Custom Image Result

Correct Predictions: 6/10

Custom Image Accuracy: 60%

## Visualizations

The notebook includes:

- Training and Validation Loss vs Epoch
- Training and Validation Accuracy vs Epoch
- Confusion Matrix
- Random Validation Predictions
- Custom Phone Image Prediction Gallery

## Model File

The trained model is saved as:

`CNN/model/CNN_RPS.pth`

## Technologies Used

- Python
- PyTorch
- Torchvision
- Scikit-learn
- Matplotlib
- Seaborn
- Google Colab
- GitHub

## Project Structure

```text
CNN/
├── dataset/
│   ├── paper_01.jpeg
│   ├── paper_02.jpeg
│   ├── rock_01.jpeg
│   ├── rock_02.jpeg
│   ├── rock_03.jpeg
│   ├── rock_04.jpeg
│   ├── scissors_01.jpeg
│   ├── scissors_02.jpeg
│   ├── scissors_03.jpeg
│   └── scissors_04.jpeg
│
├── model/
│   └── CNN_RPS.pth
│
├── CNN_RPS.ipynb
└── README.md
