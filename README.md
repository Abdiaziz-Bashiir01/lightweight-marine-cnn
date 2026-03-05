# Lightweight CNN for Marine Species Classification in Low-Resource Settings

## Overview

This repository contains the research write-up for a compact Convolutional Neural Network (CNN) developed for nine-class marine species image classification under strict computational constraints.

The primary objective of this project was to design a parameter-efficient architecture that balances predictive performance with deployability in low-resource environments. The final model contains **316,593 trainable parameters** and achieves **62.89% validation accuracy**, demonstrating that meaningful generalization can be achieved without large-scale models.

---

## Research Motivation

Marine monitoring systems often operate in computationally constrained environments where large deep learning models are impractical. While state-of-the-art architectures prioritize accuracy, they frequently neglect deployment feasibility.

This project investigates whether carefully engineered lightweight CNN architectures can provide reliable classification performance while significantly reducing parameter count and computational overhead.

---

## Model Design and Architecture

The network architecture was iteratively designed and experimentally refined to minimize parameters while maintaining stable convergence and generalization.

Key components include:

- Convolutional layers with small receptive fields
- ReLU activations
- Max-pooling for spatial downsampling
- Dropout-based regularization
- Fully connected classification head
- Softmax output layer for nine-class prediction

**Total Trainable Parameters:** 316,593

Architectural variations were systematically evaluated to analyze trade-offs between model depth, efficiency, and validation performance.

---

## Dataset and Preprocessing

The model was trained on a labeled nine-class marine species image dataset.

Preprocessing steps included:

- Image resizing and normalization
- Data augmentation (random flips and rotations)
- Controlled train-validation split

These strategies were applied to improve generalization and mitigate overfitting under limited data conditions.

---

## Experimental Setup

- Framework: PyTorch  
- Loss Function: Cross-Entropy Loss  
- Optimizer: Adam  
- Regularization: Dropout + Data Augmentation  
- Validation Accuracy: **62.89%**

Multiple experimental iterations were conducted to evaluate architectural configurations and hyperparameter settings, ensuring principled performance comparisons.

---

## Results and Contributions

This project demonstrates that:

- Compact CNN architectures can achieve competitive performance under resource constraints.
- Careful architectural tuning enables efficient trade-offs between parameter count and predictive accuracy.
- Deep learning models can be adapted for deployment in computationally limited environments without excessive complexity.

The full methodology, experimental analysis, and evaluation results are documented in the paper.

---

## Paper

The complete research write-up is available here:

📄 **[Download the Paper](https://github.com/Abdiaziz-Bashiir01/lightweight-marine-cnn/blob/main/Complete%20CNN.pdf)**

---

## Code Availability

The implementation was developed in PyTorch.  
Code and experimental details are available upon request.

This repository focuses on the research documentation and results.
