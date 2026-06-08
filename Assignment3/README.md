
# Assignment 3 – Deep Learning Experiments

## Overview
This repository contains notebooks for Assignment 3 of Applied Data Science 2026. Focus: Deep Learning architectures.  
Goal: Understand neural network behavior, experiment with hyperparameters, and analyze results.

## Notebooks

### 1. MLP – Foundations
- Implemented fully-connected neural networks for **binary classification** and **regression**.
- Experiments on: optimizers (SGD, Adam), learning rate, batch size, early stopping.
- Architecture & representation: depth, width, activation functions, weight initialization.
- Regularization: L1/L2, dropout, gradient clipping.
- Evaluation: loss curves, accuracy, RMSE/F1.
- Insight: deeper networks can learn complex patterns beyond width alone.

### 2. CNNs – Image Modeling
- Built CNNs with convolutional, pooling, and dense layers for image classification.
- Experiments on kernel size, strides, filters, pooling, and depth.
- Data augmentation: flips, rotations, crops, normalization.
- Transfer learning: pretrained VGG19, ResNet, EfficientNet; compared feature extraction vs fine-tuning.
- Visualized feature maps for interpretability.
- Insight: CNNs efficiently handle high-dimensional images; parameter sharing reduces overfitting.

### 3. RNNs – Sequence Modeling
- Implemented **Vanilla RNN, LSTM, GRU** for sequential/text data.
- Experiments: sequence length, hidden size, number of layers, bidirectionality, dropout.
- Training: early stopping, validation loss, learning curves.
- Evaluation: accuracy, F1-score, confusion matrix.
- Insight: LSTM/GRU outperform Vanilla RNN on long sequences due to gate mechanisms mitigating vanishing gradients.

### 4. ABA – Attention-Based / Transformer
- Built Transformer Encoder / MultiHeadAttention models for classification/regression.
- Compared with previous RNN/LSTM results.
- Concepts: self-attention, multi-head attention, positional encoding, computational considerations.
- Evaluation: accuracy, F1-score, confusion matrices.
- Insight: Transformers capture long-range dependencies; scalable but computationally expensive.

## Key Takeaways
- MLP: baseline for tabular data, depth helps expressivity.  
- CNN: effective for images; parameter sharing & pooling reduce overfitting.  
- RNN: LSTM/GRU better for sequences; gates mitigate vanishing gradient.  
- Transformers: excel in long-range dependencies; scalable but heavier compute.

## Research / Industry Insights (Bonus)
- Classical ML (Linear/Logistic Regression, Decision Trees) still dominant for small/structured data.  
- Deep Learning dominates unstructured data tasks (images, text, audio).  
- Transformers & LLMs increasingly deployed for NLP in industry.  
- Future trend: hybrid pipelines, wider adoption of Transformers, scalability and interpretability remain critical.  
