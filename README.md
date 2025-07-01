# Project-Local_Features_vs_CNN-for-ComputerVision

This project presents a comparative study between traditional computer vision pipelines based on handcrafted features and deep learning-based Convolutional Neural Networks (CNNs) for image classification. Experiments are conducted on two standard datasets: **Fashion-MNIST** and **CIFAR-10**.

## 📌 Overview

- Implemented local feature extraction using:
  - SIFT (DoG-based keypoints)
  - Multi-scale Harris
  - Harris-Laplace
  - A combined approach (SIFT + Harris)
- Constructed Bag-of-Words (BoW) histograms with KMeans clustering
- Classified feature histograms using Support Vector Machines (SVM)
- Designed custom CNNs of varying depth (1–6 convolutional layers) using TensorFlow/Keras
- Benchmarked accuracy, feature volume, training time, and generalization performance

## 📊 Results Summary

| Method               | Fashion-MNIST | CIFAR-10 |
|----------------------|---------------|-----------|
| Local Features (Best) | 82.5%         | 50.0%     |
| CNN (Best)            | 94.0%         | 82.0%     |

- CNNs outperformed classical methods in both accuracy and scalability
- Handcrafted methods performed competitively on grayscale, low-complexity datasets like Fashion-MNIST
- A hybrid handcrafted feature combination yielded the best result among traditional pipelines
