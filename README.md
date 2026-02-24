# 🚦 traffic-sign-detection

This project builds a **Convolutional Neural Network (CNN)** to classify traffic sign images into multiple categories using deep learning.

It demonstrates a complete **end-to-end computer vision pipeline**, including:

* Dataset download and extraction
* Image preprocessing and augmentation
* CNN model development
* Training and evaluation
* Confusion matrix and classification report
* Model saving and loading
* Prediction visualization

The objective is to accurately classify traffic sign images into their respective classes.

---

## 📌 Project Overview

* **Problem Type:** Image Classification
* **Domain:** Computer Vision / Autonomous Driving
* **Dataset:** Traffic Sign Image Dataset
* **Number of Classes:** Multiple traffic sign categories
* **Model Used:** Custom CNN (TensorFlow / Keras)
* **Test Accuracy:** **≈ 93%**

The project focuses on building an automated system capable of recognizing traffic signs from images, a key component of intelligent transportation systems. 

---

## 📊 Dataset

The dataset contains:

* Training images organized by class
* Test images with labels
* CSV files describing image paths and class IDs

Dataset link:
[https://d3ilbtxij3aepc.cloudfront.net/projects/AI-Capstone-Projects/PRAICP-1002-TrafSignDetc.zip](https://d3ilbtxij3aepc.cloudfront.net/projects/AI-Capstone-Projects/PRAICP-1002-TrafSignDetc.zip)

---

## 🔧 Data Preprocessing

* Image resizing to **32 × 32**
* Pixel normalization (rescale 1/255)
* Data augmentation:

  * Rotation
  * Zoom
  * Width & height shift
  * Shear
* Stratified train-validation split

---

## 🧠 Model Architecture

Custom CNN built using Keras:

* Conv2D → ReLU → MaxPooling
* Conv2D → ReLU → MaxPooling
* Conv2D → ReLU → MaxPooling
* Flatten layer
* Dense layer (128 neurons)
* Softmax output layer

Loss: categorical crossentropy
Optimizer: Adam

---

## 📈 Model Training

* Epochs: 5
* Batch size: 32
* Validation set used during training
* Training and validation accuracy visualized

---

## 📊 Model Evaluation

Evaluation performed using:

* Test accuracy
* Confusion matrix
* Classification report
* Sample prediction visualization

### 🏆 Result

**Test Accuracy ≈ 93%**

The model shows strong classification capability across traffic sign classes.

---

## 🔮 Prediction

The trained CNN predicts traffic sign class labels for unseen images and displays predicted vs actual results.

---

## 💾 Model Saving & Loading

The trained model is saved as:

```
traffic_sign_classifier.h5
```

It can be reloaded for inference without retraining.

---

## ⚠️ Challenges

* Dataset extraction issues and path handling
* Ensuring correct image generator configuration
* Class imbalance and visually similar signs
* Training with limited epochs

---

## 🚀 Future Improvements

* Transfer learning (ResNet / EfficientNet / MobileNet)
* Hyperparameter tuning
* Longer training with early stopping
* Advanced augmentation strategies
* Class imbalance handling
* Real-time inference pipeline

---

## 🚀 How to Run

```bash
git clone https://github.com/SyedHussain23/traffic-sign-detection
cd traffic-sign-detection
pip install -r requirements.txt
jupyter notebook traffic-sign-detection.ipynb
```

---

## 👨‍💻 Author

**Syed Hussain Abdul Hakeem**

* GitHub: [https://github.com/SyedHussain23](https://github.com/SyedHussain23)
* LinkedIn: [https://www.linkedin.com/in/syed-hussain-abdul-hakeem](https://www.linkedin.com/in/syed-hussain-abdul-hakeem)

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐.
