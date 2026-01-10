# Apple Leaf Disease Classification (Comparative Study) 🍎🌿

![Status](https://img.shields.io/badge/Status-Manuscript_Ready-yellow)
![Best Accuracy](https://img.shields.io/badge/Best_Accuracy-96%25-success)
![Classes](https://img.shields.io/badge/Classes-3_(Healthy,_Scab,_Rust)-blue)

## 📌 Project Overview
This research project focuses on the multi-class classification of apple leaves into **3 categories: Healthy, Scab, and Rust**.
The primary goal of this work is to benchmark different Deep Learning architectures to find the most accurate model for agricultural disease detection.

> **Current Scope:** This repository contains the training and validation code to calculate and compare model accuracy. Real-time inference (prediction on single image) is currently under development.

## 🔬 Comparative Analysis (The Surprise Result)
We trained 4 different models. Surprisingly, our lightweight **Custom CNN** matched the performance of the heavy **ResNet50**, while MobileNetV2 significantly underperformed on this specific dataset.

| Rank | Model Architecture | Test Accuracy | Research Verdict |
|------|-------------------|---------------------|---------------------|
| 🥇 | **Custom CNN** | **96.0%** | ✅ **Best Model (Lightweight & Accurate)** |
| 🥈 | **ResNet50** | **96.0%** | High Accuracy but Computationally Heavy |
| 🥉 | EfficientNetB0 | 95.0% | Very Competitive |
| 4 | MobileNetV2 | 67.0% | ❌ Failed to capture features effectively |

## 🛠️ Dataset & Methodology
- **Classes:** 3 (Healthy, Scab, Rust).
- **Preprocessing:** Images resized and normalized.
- **Strategy:** Compared Transfer Learning (ResNet, EfficientNet, MobileNet) against a Custom CNN built from scratch.

## 📝 Research Status
**Manuscript Drafted:** *Benchmarking CNN Architectures for Apple Leaf Disease Diagnosis.*
*(Status: Ready for Submission).*

## 👨‍💻 Tech Stack
- **Deep Learning:** TensorFlow, Keras
- **Visualization:** Matplotlib (for accuracy/loss graphs)
- **Data Handling:** NumPy, Pandas
