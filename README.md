# Denoising-Images-with-Autoencoders
# 🧠 Image Denoising using Autoencoders (CIFAR-10)

This project demonstrates how deep learning can be used to remove noise from images using a Convolutional Autoencoder.

---

## 📌 Overview
Autoencoders are neural networks designed to learn compressed representations of data. In this project, we train an autoencoder to reconstruct clean images from noisy inputs.

---

## 📊 Dataset
- CIFAR-10 dataset (32x32 RGB images)
- Images normalized to [0,1]
- Gaussian noise added to simulate real-world noise

---

## ⚙️ Tech Stack
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib

---

## 🏗️ Model Architecture

### Encoder:
- Conv2D → ReLU
- MaxPooling
- Conv2D → ReLU
- MaxPooling

### Decoder:
- Conv2D → ReLU
- UpSampling
- Conv2D → ReLU
- UpSampling
- Conv2D → Sigmoid

---

## 📈 Results

The model successfully reconstructs clean images from noisy inputs.

| Noisy Image | Denoised Image |
|------------|---------------|
| ![](outputs/noisy.png) | ![](outputs/denoised.png) |

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
