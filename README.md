# TransferLearning-MobileNet-v2

Transfer Learning with MobileNet-v2 for Alpaca Classification
This repository contains a TensorFlow/Keras implementation of transfer learning using MobileNet-v2 for binary image classification (Alpaca vs. Not Alpaca). The project demonstrates how to adapt a pre-trained model to a custom dataset through feature extraction and fine-tuning.

# Project Overview
- The included Jupyter Notebook guides you through:

- Loading and preprocessing a custom dataset

- Applying data augmentation to improve generalization

- Transfer learning steps:

  - Freezing the base model (MobileNet-v2) and training a custom classification head

  - Fine-tuning the top layers of the base model for improved accuracy

- Evaluating model performance with metrics and visualizations



# Features
- Built with TensorFlow 2.x and Keras API

- Uses MobileNet-v2 (pre-trained on ImageNet) as a feature extractor

- Two-stage training:

  - Stage 1: Train only the custom head (base model frozen)

  - Stage 2: Fine-tune top layers of the base model

- Includes data augmentation:

  - Random rotation

  - Zoom

  - Horizontal flip

- Visualizations for training and validation loss and accuracy




# Dataset

The dataset used is the Alpaca Classifier Dataset from Kaggle:
🔗 [Kaggle Dataset Source](https://www.kaggle.com/datasets/sid4sal/alpaca-dataset-small)

- Alpaca: 142 images

- Not Alpaca: 185 images

Total: 327 images

The dataset is used for binary classification and is split into training and validation sets. All images are resized and normalized during preprocessing.
