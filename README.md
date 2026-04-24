# 🚗 Intelligent Number Plate Recognition System

### (CV + CNN + Transformer-based Approach with Cloud Deployment)

---

## 📌 Overview

This project presents an **end-to-end Automatic Number Plate Recognition (ANPR) system** designed using a hybrid approach combining:

* Classical **Computer Vision techniques**
* **Convolutional Neural Networks (CNN)**
* **Sequence modeling (Transformer / RNN-based OCR)**

The system detects, extracts, and recognizes vehicle number plates from images and provides **analytics for parking management**.

---

## 🎯 Objectives

* Detect number plates from vehicle images
* Extract plate region using CV techniques
* Recognize characters using deep learning
* Provide insights for parking analytics
* Enable real-time inference and cloud deployment

---

## 🧠 System Architecture

```
Input Image
     ↓
CV Preprocessing (Segmentation + Edge Detection + Corners)
     ↓
Plate Localization (ROI Extraction)
     ↓
CNN Feature Extraction (EfficientNet / ResNet)
     ↓
Sequence Modeling (RNN / Transformer OCR)
     ↓
Text Output (Plate Number)
     ↓
Analytics + Storage + Dashboard
```

---

## 📂 Dataset

* **Indian Number Plate Dataset** (Kaggle)
* Split:

  * Training: 70%
  * Validation: 15%
  * Test: 15%

Additional:

* Real-world parking images for final evaluation

---

## ⚙️ Technologies Used

* **Python**
* **OpenCV** (Image processing)
* **PyTorch** (Deep Learning)
* **Albumentations** (Data augmentation)
* **Matplotlib** (Visualization)

Deployment:

* **FastAPI** (REST API)
* **Docker** (Containerization)
* **Google Cloud Platform (GCP)**

---

## 🔍 Key Features

### 🔹 1. Computer Vision Preprocessing

* Grayscale conversion
* Thresholding
* Edge detection (Canny)
* Contour detection
* Corner detection (Harris)

### 🔹 2. Plate Localization

* Region of Interest (ROI) extraction
* Bounding box detection
* Optional perspective correction

### 🔹 3. Deep Learning Model

* CNN Backbone: EfficientNet / ResNet
* Sequence Model: RNN / Transformer
* Output: Character sequence

### 🔹 4. Training

* Loss Function: CrossEntropy / CTC (initially explored)
* Optimization: Adam
* Gradient clipping for stability

### 🔹 5. Post-processing

* Duplicate detection (Levenshtein distance)
* Plate validation
* Data logging

### 🔹 6. Analytics

* Parking zone mapping
* Timestamp tracking
* Occupancy estimation

---

## 🧪 Results

* Successful detection of number plates from vehicle images
* Accurate character recognition under controlled conditions
* Robust performance with preprocessing improvements

*(Add accuracy numbers if available)*

---

## 🎥 Real-Time Processing

* Frame-by-frame video processing
* Vehicle tracking across frames
* Plate recognition in dynamic scenes

---

## ☁️ Deployment

* Model served using **FastAPI**
* Containerized using **Docker**
* Deployed on **Google Cloud Platform**

Optional:

* Kubernetes for scalability

---

## 🔁 CI/CD Pipeline

* Version control using Git + GitHub
* Automated workflows using GitHub Actions:

  * Model training
  * Testing
  * Deployment

---

## 📊 Future Improvements

* Improve OCR accuracy using full Transformer models
* Add multi-plate detection
* Enhance real-time tracking
* Integrate database for large-scale analytics
* Deploy scalable Kubernetes-based system

---

## 📸 Sample Output

```
Input Image → Detected Plate → Predicted Text
Car Image   → Bounding Box  → MH12AB1234
```

---

## 👨‍💻 Author

**Harsh Mulimani**
Computer Science (AI & ML)

---

## 📎 Notes

* Initial implementation used CTC Loss but was replaced with CrossEntropy for stability
* Focus was given to **end-to-end pipeline and system design**

---

## ⭐ Conclusion

This project demonstrates a **complete intelligent vision system**, integrating:

* Classical CV techniques
* Deep learning models
* Real-time processing
* Cloud deployment

It provides a scalable solution for **smart parking and traffic monitoring systems**.

---
