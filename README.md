
# Brain Tumor Detection using Deep Learning (VGG16)

# Overview

This project focuses on detecting and classifying brain tumors from MRI images using Deep Learning techniques. The model is built using transfer learning with VGG16 and trained on brain tumor datasets.

The system supports:

 Multi-class classification (Glioma, Meningioma, Pituitary, No Tumor)
 Binary classification (Tumor vs No Tumor)



# Objectives

Classify brain MRI images into tumor categories
 Improve model performance using transfer learning and fine-tuning
 Apply data augmentation to enhance generalization
 Evaluate performance on unseen test data


# Dataset

The dataset was collected from Kaggle.

# Classes:

 Glioma
 Meningioma
 Pituitary
 No Tumor

# Technologies Used

 Python
 TensorFlow / Keras
 OpenCV
 NumPy / Matplotlib
 Scikit-learn


# Data Preprocessing

Image resizing to 224x224
 Normalization (rescaling pixel values)
 Data augmentation:
   Rotation
   Zoom
   Width & height shift
   Horizontal & vertical flip


# Model Architecture

 Pretrained VGG16 (ImageNet weights)
 Frozen base layers
 Custom classification head:
    Global Average Pooling
    Dense layer with Softmax / Sigmoid


# Training Strategy

1. Train only the top layers
2. Apply Early Stopping to avoid overfitting
3. Fine-tune last layers with lower learning rate



# Results

 Multi-class Accuracy: ~94% after fine-tuning
 Binary Classification Accuracy: ~92%


# Project Structure

brain-tumor-detection/
│── data/
│── train/
│── test/
│── models/
│── notebooks/
│── README.md



# How to Run:

# Install dependencies

pip install -r requirements.txt

# Run training

python train.py

# Evaluate model

python evaluate.py


# Challenges

  Overfitting due to limited data
  Class imbalance
  Improving generalization


# Future Improvements

  Deploy model using Flask API
  Add Grad-CAM for explainability
  Use advanced architectures (ResNet, EfficientNet)


# Author
Salma Khairy & Sara Ehab
AI & Data Science Students – Zewail City
