# Geolocation Classifier Using CNNs

A deep learning project that classifies images based on their **geolocation** (continent or country) using **Convolutional Neural Networks (CNNs)**. Built as a part of a semesterial project.

---

## 📌 Overview

The objective of this project is to **build and optimize a deep learning model** that can predict the **geographical location** of a given image. The classification is done on both the **country** and **continent** level.

---

## 🧠 Learning Journey

We started with minimal knowledge of CNNs and transfer learning. Through self-study and hands-on experimentation, we:

- Researched the fundamentals of Deep Learning.
- Explored CNN architectures and Transfer Learning.
- Learned and implemented optimization techniques.

---

## 📦 Dataset

- **25,000 images** with 640x640 resolution.
- Sourced from **Kaggle** and the **Google Street View API**.
- Annotated with **geolocation metadata** (CSV files containing image IDs and location details).

---

## ⚙️ Data Preprocessing

- Resized all images to a uniform shape.
- Applied **data augmentation** (rotation, zoom, shear).
- Normalized image pixel values.
- Filtered based on sample size thresholds.
- Split into **training**, **validation**, and **test** datasets.

---

## 🏗️ Model Development

We built and experimented with the following architectures:

### ✅ Pretrained Models Used
- **MobileNetV2** – Fast and efficient.
- **VGG16** – High accuracy, deeper layers.
- **ResNet50** – Strong generalization.

### ⚙️ Key Techniques
- Transfer Learning: Used pretrained weights, fine-tuned top layers.
- Added custom **Dense** and **Dropout** layers.
- Optimized training with **Early Stopping**, **ReduceLROnPlateau**, and efficient data loading.

---

## 🔧 Hyperparameter Tuning

We experimented with:
- Learning rates and batch sizes.
- Dropout rates to reduce overfitting.
- Data augmentation parameters.
- Loss functions and callbacks for training efficiency.

---

## 🚀 Performance Results

| Task                        | Model       | Test Accuracy |
|----------------------------|-------------|---------------|
| Country Classification (5) | VGG16       | 72.0%         |
| Country Classification (10)| VGG16       | 59.8%         |
| Country Classification (10)| ResNet50    | 51.7%         |
| Continent Classification   | MobileNetV2 | 64.8%         |
| Continent Classification   | VGG16       | 67.4%         |

---

## 💻 Optimization

- Used **GPU acceleration** via WSL + CUDA for efficient training.
- Reduced CPU overhead with optimized data loaders.

