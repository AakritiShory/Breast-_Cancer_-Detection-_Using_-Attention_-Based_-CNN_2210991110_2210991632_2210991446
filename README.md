# 🩺 Breast Cancer Detection using Attention-Based CNN

Early diagnosis can make a major difference in breast cancer treatment outcomes. This project explores the use of deep learning for automated breast cancer detection by combining Convolutional Neural Networks (CNNs) with an attention mechanism that helps the model focus on important tumor regions in medical images.

Instead of processing the entire image with equal importance, the attention module guides the network toward meaningful patterns and suppresses irrelevant background information. The goal is to improve classification performance while creating a more reliable computer-aided diagnostic system.

---

## 🚀 Project Overview

The proposed workflow follows these stages:

Input Image → Preprocessing → CNN Feature Extraction → Attention Module → Classification Output

The system performs binary classification and predicts whether a medical image belongs to:

- Benign
- Malignant

---

## ✨ Features

✔ Medical image preprocessing pipeline  
✔ Transfer learning-based CNN architecture  
✔ Attention mechanism for feature refinement  
✔ Binary classification using sigmoid activation  
✔ Data augmentation for better generalization  
✔ Performance evaluation metrics  
✔ Training and validation visualization  

---

## 🧠 Methodology

The model follows a deep learning pipeline designed for medical image analysis.

### Data Preprocessing
Medical images undergo several preprocessing steps before training:

- Image resizing (224 × 224)
- Normalization
- Contrast enhancement
- Noise reduction
- Data augmentation
  - Rotation
  - Horizontal flip
  - Zoom
  - Shift

### Feature Extraction
A CNN backbone extracts hierarchical spatial features from input images.

Feature extraction:

F = CNN(X)

where:

- X → Input image
- F → Feature map

### Attention Mechanism

The attention module assigns importance weights to extracted features:

F' = F · A

where:

- F → Original feature map
- A → Attention weights
- F' → Refined feature map

The model learns to focus on tumor-relevant regions while suppressing irrelevant information.

### Classification

The refined features pass through fully connected layers for final prediction:

Y = σ(WF' + b)

where:

- Y → Predicted class
- W → Weight matrix
- b → Bias
- σ → Sigmoid activation function

---

## ⚙️ Training Configuration

| Parameter | Value |
|-----------|--------|
| Optimizer | Adam |
| Loss Function | Binary Cross Entropy |
| Learning Rate | 0.001 |
| Batch Size | 32 |
| Epochs | 40–50 |
| Early Stopping | Enabled |

---

## 📊 Evaluation Metrics

Model performance is evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 📁 Project Structure
Breast-Cancer-Detection/
│
├── dataset/
├── preprocessing/
├── models/
├── notebooks/
├── results/
├── images/
├── train.py
├── evaluate.py
├── requirements.txt
├── README.md


---

## 📈 Sample Outputs

The repository includes:

- Training Accuracy Curve
- Training Loss Curve
- Confusion Matrix
- Classification Results
- Model Performance Analysis

(Add screenshots here after training)

---

## 💡 Future Improvements

There are several directions for extending this work:

- Integrating larger datasets
- Exploring transformer-based architectures
- Improving interpretability techniques
- Real-time clinical deployment
- Multi-class tumor classification

---

## 🎯 Research Objective

To develop an intelligent and reliable computer-aided system capable of assisting healthcare professionals in early breast cancer detection through attention-enhanced deep learning techniques.

---

## 👨‍💻 Authors

Aakriti Shory, 
Harshit,
Bhoomika,
Isha Kansal
Department of Computer Science  
Chitkara University  

---

*"AI in healthcare is not about replacing doctors; it is about building tools that help them make faster and more informed decisions."*

