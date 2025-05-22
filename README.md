# Lung Tumor Classification Using DenseNet121

## 🚀 Project Overview

This project implements a **state-of-the-art deep learning pipeline** for classifying lung tumors as either **benign** or **malignant** using the powerful DenseNet121 architecture. Leveraging transfer learning and advanced data augmentation, the model achieves high accuracy on medical X-ray images, helping radiologists make faster and more reliable diagnoses.

---

## 🔍 Dataset

- The dataset consists of chest X-ray images stored in Google Drive.
- Metadata is stored in CSV files, detailing image filenames and corresponding labels (`benign` or `malignant`).
- Stratified K-Fold cross-validation (K=10) is applied to ensure balanced and robust evaluation.

---

## ⚙️ Features

- **DenseNet121** pretrained on ImageNet, fine-tuned for binary tumor classification.
- Custom dataset loader with real-time image transformations:
  - Resizing to 224x224
  - Normalization (mean=0.5, std=0.5)
- Data augmentation pipeline (optional, can be added for training).
- Training loop with:
  - Cross-entropy loss
  - Adam optimizer with learning rate scheduling
- Validation and test phases with detailed classification reports and confusion matrices.
- Visualization of training loss and accuracy over epochs.
- Model saving and loading to/from Google Drive.
- Stratified K-Fold evaluation for reliable performance metrics.

---



