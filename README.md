# Lightweight Cassava Disease Detection for Edge Devices

## 📌 Project Overview
Agriculture is the backbone of Cambodia's economy, yet farmers lose significant yield to viral diseases like **Cassava Mosaic Disease (CMD)** due to delayed diagnosis.

This project develops a **lightweight Deep Learning model (MobileNetV2/EfficientNet-Lite)** optimized for offline deployment on low-cost Android devices. The goal is to provide real-time, internet-free disease diagnosis for rural farmers.

## 🎯 Research Objectives
1.  **Efficiency:** Fine-tune `MobileNetV2` to achieve >90% accuracy on the Cassava Leaf Disease dataset.
2.  **Optimization:** Apply **Post-Training Quantization (PTQ)** to reduce model size to under 5MB (TFLite format).
3.  **Deployment:** Prototype an offline Android application for field testing.

## 🛠️ Tech Stack
* **Core Framework:** Python, TensorFlow / Keras
* **Model Architecture:** MobileNetV2 (Transfer Learning)
* **Optimization:** TensorFlow Lite (Quantization)
* **Data Source:** [Kaggle Cassava Leaf Disease Classification](https://www.kaggle.com/c/cassava-leaf-disease-classification)

## 📊 Methodology
* **Step 1: Data Preprocessing:** Image augmentation (rotation, zoom) to simulate real-world field conditions.
* **Step 2: Transfer Learning:** Freezing the base layers of MobileNetV2 (ImageNet weights) and training a custom classification head.
* **Step 3: Quantization:** Converting the `.h5` model to `.tflite` to minimize latency on ARM processors.

## 🚀 How to Run (Google Colab)
1.  Clone this repository.
2.  Open `notebooks/train_model.ipynb` in Google Colab.
3.  Set Runtime to **T4 GPU**.
4.  Run all cells to download data and train the model.

## 🔮 Future Work (Research Proposal)
This project serves as the preliminary work for a Master's research proposal focusing on **"Federated Learning for Privacy-Preserving Agricultural AI in Southeast Asia."**
