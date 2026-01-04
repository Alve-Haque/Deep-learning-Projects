
# Fashion Image Classification & Visual Search System (PyTorch)

## Overview
This repository contains a **production-oriented deep learning system** for **fashion image classification** and **visual similarity search**, implemented using **PyTorch**. The project emphasizes **efficient CNN architectures**, **scalable training pipelines**, and **metric learning**, mirroring real-world machine learning engineering workflows.

The solution is designed with **deployability, modularity, and performance** in mind.

---

## Key Engineering Contributions
- Implemented a **MobileNet-style CNN** with inverted residual blocks
- Built a **custom training pipeline** with schedulers and optimizers
- Designed a **triplet-based metric learning system** for visual search
- Structured code for **reuse, testing, and extension**

---

## System Architecture

### Classification Model
- Lightweight CNN backbone inspired by **MobileNetV2**
- Depthwise separable convolutions for computational efficiency
- Residual connections for stable and fast convergence

### Visual Search Model
- Siamese-style encoder with shared weights
- Embedding-based similarity learning using **Triplet Margin Loss**
- Euclidean distance–based nearest neighbor retrieval

---

## Training Details

### Classification
| Component | Value |
|---------|------|
| Optimizer | Adam |
| Learning Rate | 0.01 |
| Scheduler | StepLR |
| Loss Function | Cross Entropy |
| Epochs | 5 |

### Metric Learning
| Component | Value |
|---------|------|
| Optimizer | AdamW |
| Learning Rate | 0.001 |
| Loss Function | TripletMarginLoss |
| Epochs | 5 |

---

## Engineering Strengths Demonstrated
- PyTorch model engineering and optimization
- Efficient CNN architecture design
- Custom dataset abstractions and samplers
- Modular training, evaluation, and inference pipelines
- Realistic ML system design for e-commerce and vision applications

---

## Project Structure
```
├── C3M1_Assignment.ipynb
├── helper_utils.py
├── unittests.py
├── data/
└── README.md
```

---

## Applications
- Fashion product classification
- Visual search engines for e-commerce
- Recommendation systems
- Edge and mobile AI deployments

---

## Ideal For Roles
- Machine Learning Engineer
- Applied ML Engineer
- AI Engineer

---

## How to Run
```bash
pip install torch torchvision numpy matplotlib
jupyter notebook C3M1_Assignment.ipynb
```

---

## Notes for Recruiters
This project demonstrates the ability to design and implement **efficient, scalable, and production-ready deep learning systems**, combining supervised learning and metric learning techniques commonly used in real-world computer vision applications.
