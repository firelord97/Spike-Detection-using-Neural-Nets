# 🧠 Spike Detection Using Neural Networks

This repository contains the implementation and analysis of neural network methods for spike detection in high-density Multi-Electrode Array (MEA) data. The project explores the application of a Multi-Layer Perceptron (MLP) for spike detection, comparing its performance across different levels of noise in simulated neural data.

---

## 📑 Table of Contents

1. [Introduction](#introduction)
2. [Background](#-background)
3. [Methodology](#-methodology)
4. [Results](#-results)
5. [Discussion](#-discussion)
6. [Future Work](#-future-work)
7. [References](#-references)

---

## Introduction

Spike detection is crucial for understanding neural activity. This project focuses on developing a neural network-based approach to detect spikes in biophysically-realistic simulated data from MEAs. The model aims to provide efficient and scalable spike detection under varying noise conditions.

---

## Background

Spikes, or action potentials, are fundamental units of communication in the nervous system. Traditional methods for spike detection often rely on threshold-based or template-based techniques, which may require manual tuning. With the advancement of high-density MEAs, there is a need for automated and robust detection methods, leading to the exploration of neural networks.

---

## Methodology

1. **Data Preparation**: The data used in this project consists of simulated MEA recordings generated with the MEArec library, including datasets with different noise levels.
2. **Model Design**: A basic MLP with two hidden layers was implemented to classify 50-frame snippets of voltage data as containing a spike or not.
3. **Training and Testing**: The model was trained on snippets with known spikes and evaluated on datasets with varying noise levels. Snippet centering techniques and performance evaluation methods were also applied.

---

## Results

1. **Low-Noise Dataset**: The MLP achieved high accuracy in detecting spikes, with fewer false positives compared to a baseline threshold classifier.
2. **High-Noise Dataset**: Performance decreased in noisier data, but the MLP still outperformed the baseline method. False positives increased due to noise-induced artifacts.
3. **Model Variations**: Experiments with snippet lengths and network complexity (number of layers and neurons) demonstrated trade-offs between speed and accuracy.

---

## Discussion

The MLP-based approach showed promise for efficient spike detection, especially in low-noise conditions. However, challenges remain in spike sorting (assigning spikes to specific neurons) in high-noise environments. The project highlights the potential of neural networks in automating spike detection but also points to limitations with basic architectures.

---

## Future Work

1. **Model Optimization**: Implementing more sophisticated neural network architectures like Convolutional Neural Networks (CNNs) and using Bayesian optimization for hyperparameters.
2. **Real Data Application**: Extending the model's application to real neural recording datasets to evaluate generalizability.
3. **Spike Sorting Improvements**: Enhancing spike sorting accuracy through advanced network designs and multi-step detection processes.

---

## References

1. **Spike Sorting Techniques**: Literature on traditional methods and neural network applications.
2. **MEAs**: Background on Multi-Electrode Arrays and their role in neural data collection.
3. **Machine Learning Frameworks**: Scikit-learn and other tools used in this project.

---

