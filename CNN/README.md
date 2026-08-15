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
