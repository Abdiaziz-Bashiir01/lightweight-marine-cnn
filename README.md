# Lightweight CNN for Marine Species Classification in Low-Resource Settings

## Overview

This project presents a compact Convolutional Neural Network (CNN) designed for nine-class marine species image classification in low-resource environments. The primary objective was to balance predictive accuracy with computational efficiency, enabling deployment on hardware with limited processing power and memory capacity.

The final model contains **316,593 trainable parameters** and achieves **62.89% validation accuracy**, demonstrating that meaningful performance can be achieved under strict resource constraints.

---

## Motivation

Many real-world marine monitoring systems operate in environments with limited computational resources. Traditional deep learning models are often too large for deployment in such settings. This project explores parameter-efficient architecture design while maintaining reasonable generalization performance.

---

## Model Architecture

The network is a lightweight CNN composed of:

- Convolutional layers with small kernel sizes
- ReLU activations
- Max-pooling layers for spatial downsampling
- Dropout for regularization
- Fully connected classification head
- Softmax output layer (9 classes)

The architecture was iteratively optimized to minimize parameter count while preserving classification performance.

**Total Parameters:** 316,593

---

## Dataset

The model was trained on a nine-class marine species image dataset.

Classes include various marine organisms categorized for supervised classification.  
Data preprocessing included:

- Image resizing
- Normalization
- Data augmentation (random flips, rotations)
- Train-validation split

---

## Training Details

- Framework: PyTorch
- Loss Function: Cross-Entropy Loss
- Optimizer: Adam
- Regularization: Dropout + Data Augmentation
- Validation Accuracy: **62.89%**

Multiple architectural variations were tested to evaluate trade-offs between:

- Model depth
- Parameter efficiency
- Training time
- Validation performance

---

## Results

The final model demonstrates stable convergence and reliable generalization under limited computational resources.

Example evaluation outputs and training curves are available in the `/results` directory.

---

## Note on Code Availability

The implementation code is available upon request. 
This repository focuses on the research write-up and experimental results.
