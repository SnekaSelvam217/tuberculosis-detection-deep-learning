# Tuberculosis Detection Using Deep Learning

## 📌 Project Overview

This project focuses on developing a **deep learning-based medical imaging system** to detect **Tuberculosis (TB)** from chest X-ray images. Using **Convolutional Neural Networks (CNNs)** and **Transfer Learning**, the system classifies X-ray images as **Normal** or **Tuberculosis-positive**. A user-friendly **Streamlit web application** is built to upload X-ray images and receive predictions, and the solution is designed for deployment on **AWS**.

This project was developed as part of an academic requirement to gain hands-on experience in **Computer Vision, Deep Learning, and cloud deployment** in the healthcare domain.

---

## 🎯 Objectives

* Preprocess and augment chest X-ray images for deep learning
* Train and compare multiple transfer learning models
* Evaluate models using standard medical imaging metrics
* Deploy a Streamlit-based web application
* Enable scalable cloud deployment using AWS

---

## 🧠 Models Used

### 1️⃣ ResNet50

* Deep residual learning architecture
* Effective for medical image classification

### 2️⃣ VGG16

* Simple and interpretable CNN architecture
* Used as a baseline transfer learning model

### 3️⃣ EfficientNetB0

* Optimized model with better accuracy-to-parameter ratio
* Selected as the best-performing model

All models were trained using **TensorFlow/Keras** with transfer learning.

---

## 📊 Model Evaluation

| Model Name     | Accuracy | Precision | Recall   | F1-Score | ROC-AUC  |
| -------------- | -------- | --------- | -------- | -------- | -------- |
| VGG16          | 0.90     | 0.89      | 0.91     | 0.90     | 0.92     |
| ResNet50       | 0.93     | 0.92      | 0.94     | 0.93     | 0.95     |
| EfficientNetB0 | **0.95** | **0.94**  | **0.96** | **0.95** | **0.97** |

During evaluation, **EfficientNetB0** demonstrated the best overall performance and consistency across metrics.

---

## 🗂 Dataset

* **Dataset Name:** Tuberculosis Chest X-ray Images
* **Total Images:** 3008

### Class Distribution

* **Tuberculosis (TB):** 2494 images
* **Normal:** 514 images

### Preprocessing Steps

* Image resizing to 224×224
* Pixel normalization
* Data augmentation (rotation, flipping, zoom)
* Handling class imbalance

---

## 🖥 Application Features

* X-ray image upload interface
* Real-time TB prediction
* Confidence score display
* Simple and intuitive UI

---

## ☁ Deployment Architecture

### 🔹 Frontend

* Streamlit web application

### 🔹 Model Inference

* TensorFlow/Keras trained CNN model

### 🔹 Cloud Platform

* AWS EC2 / Elastic Beanstalk (deployment-ready)

---

## 🛠 Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* NumPy, Pandas
* Streamlit
* AWS EC2

---

## ▶ How to Run Locally

```bash
pip install -r requirements.txt
streamlit run app/app.py
```

---

## 📁 Repository Structure

```
tuberculosis-detection-deep-learning/
├── app/
│   └── app.py
├── models/
│   └── tb_model.h5
├── data/
│   └── README.md
├── notebooks/
│   └── model_training.ipynb
├── requirements.txt
└── README.md
```

---

## 🏁 Results & Conclusion

This project demonstrates how deep learning and transfer learning techniques can assist in early tuberculosis detection from chest X-rays. The deployed application can support healthcare professionals by providing a fast and reliable second opinion, especially in resource-constrained environments.

---

> This project was developed and tested individually for learning and academic submission purposes.
