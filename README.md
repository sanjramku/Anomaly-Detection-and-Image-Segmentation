Anomaly Odyssey (Computer Vision)

## Overview
This repository contains my implementation for "Task 2: Anomaly Odyssey," a computer vision challenge focused on Anomaly Detection and Image Segmentation. The primary objective of this task is to build robust models capable of identifying and segmenting anomalies in image data using the MVTec AD dataset.

## Task Guidelines & Constraints
This project was developed strictly adhering to the following AI Guild guidelines:
* **No Pretrained Anomaly Models:** The use of models pretrained on MVTec AD or any other specific anomaly detection datasets is not permitted.
* **Independent Training:** While replicating architectures from established research papers is allowed, all models were trained or fine-tuned independently from scratch.
* **No External Data:** The models are trained exclusively on the provided dataset.
* **Solo Project:** This is an individual task with performance tracked via a live leaderboard.

## Dataset & Evaluation
* **Dataset:** MVTec Anomaly Detection (MVTec AD) Dataset.
* **Metrics:** Model performance is primarily evaluated using the Area Under the Receiver Operating Characteristic Curve (AUC-ROC), focusing on both the accurate classification of an anomaly and its precise pixel-level localization.

## Core Methodologies & Architectures
To tackle this challenge, the pipeline explores several advanced computer vision techniques and architectures:

* **Image Processing & Feature Extraction:** Utilizing OpenCV and Torchvision transforms for noise removal, image preprocessing, and feature matching.
* **Convolutional Neural Networks (CNNs):** Building and training custom CNN architectures for local feature extraction, alongside visualizing network focus areas using tools like Grad-CAM.
* **Image Segmentation:** Implementing U-Net architectures in PyTorch to generate precise masks of the detected anomalies.
* **Vision Transformers (ViT):** Leveraging self-attention mechanisms to capture global context and long-range dependencies within the images.
* **Generative Models:** Exploring Autoencoders, Variational Autoencoders (VAEs), Generative Adversarial Networks (GANs), and Diffusion models to learn the baseline distribution of "normal" images and mathematically flag deviations as anomalies.
* **Unsupervised & Self-Supervised Learning:** Applying techniques like Knowledge Distillation, DINO, and K-Nearest Neighbors to build robust representations without relying heavily on labeled anomaly data.
