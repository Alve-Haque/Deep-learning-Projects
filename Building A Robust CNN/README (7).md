# Overcoming Overfitting: Building a Robust Convolutional Neural Network (CNN)

## 📌 Project Overview

Overfitting is one of the most persistent challenges in deep learning, particularly when training convolutional neural networks on limited or complex datasets. This project demonstrates a systematic and practical approach to building a robust CNN that generalizes well by combining:

- A carefully designed data pipeline  
- Strong regularization techniques  
- A modular CNN architecture  
- A clean and reproducible training and validation workflow  

The project uses a subset of the CIFAR-100 dataset and focuses on improving model generalization rather than merely increasing training accuracy.

---

## 🎯 Objectives

The key goals of this project are to:

- Reduce overfitting through data augmentation, dropout, and weight decay  
- Build a clean, modular CNN architecture that is easy to extend  
- Implement a reliable training and validation loop  
- Track and retain the best-performing model based on validation accuracy  
- Provide a strong learning reference for building production-ready CNNs  

---

## 🧠 Dataset

- Dataset: CIFAR-100 (subset)  
- Task: Multi-class image classification (15 selected classes)  
- Input size: 32 × 32 RGB images  

The dataset is intentionally constrained to highlight the effects of overfitting and the importance of proper regularization.

---

## 🔧 Project Structure & Key Components

### 1️⃣ Data Pipeline Enhancement

A strong data pipeline is the foundation of a robust model.

Key techniques used:
- Dataset-specific normalization (mean & standard deviation)
- Data augmentation including:
  - Random horizontal flips
  - Random rotations
- Separate transformations for training (augmented) and validation (non-augmented)

---

### 2️⃣ Modular CNN Architecture

The CNN is built using a modular design, making it both readable and extensible.

Architectural highlights:
- Reusable convolutional blocks
- Batch Normalization for training stability
- ReLU activations
- Max Pooling for spatial downsampling
- Dropout layers to reduce feature co-adaptation
- Fully connected classifier head sized for 15 classes

---

### 3️⃣ Regularization Strategies

To combat overfitting, the following strategies are employed:

- Dropout
- Weight Decay (L2 Regularization)
- Data Augmentation

---

### 4️⃣ Training & Validation Workflow

Key features:
- Clear separation between training and validation logic
- GPU/CPU device abstraction
- Best model checkpointing based on validation accuracy
- Accuracy tracking across epochs

---

## 📈 Results & Outcomes

- Improved validation accuracy compared to a baseline CNN
- Reduced gap between training and validation performance
- Stable convergence behavior

---

## 🚀 How to Run the Project

### Prerequisites
- Python 3.x
- PyTorch
- torchvision
- NumPy
- Matplotlib

### Steps
```bash
git clone <repository-url>
cd <repository-name>
jupyter notebook Building_a_robust_CNN.ipynb
```

---

## 📚 Learning Takeaways

- Understanding overfitting in CNNs
- Effective use of data augmentation
- Modular deep learning code design
- Best practices for CNN training pipelines

---

## 🏁 Conclusion

This project demonstrates how principled model design and regularization techniques can significantly improve CNN generalization and reliability.
