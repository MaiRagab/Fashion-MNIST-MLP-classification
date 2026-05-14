# 👩‍💻 Mai Ragab Khalaf >>>  Neural Network (MLP) Project

## 📌 Project Overview
This project implements a Multilayer Perceptron (MLP) using PyTorch for Fashion-MNIST image classification.  
The goal is to classify images of clothing items into 10 categories.

Two experiments were conducted to analyze the effect of learning rate and network depth on performance.

---

## 📊 Dataset
- Fashion-MNIST dataset
- 10 classes of clothing images
- 28x28 grayscale images
- Loaded using torchvision

---

## ⚙️ Preprocessing
- Converted images to tensors
- Normalization applied
- Dataset split into:
  - Training set
  - Validation set (80/20 split)
  - Test set

---

## 🧠 Model Architecture

### Experiment 1
- Input: Flatten (784)
- Hidden layers: 2 (256, 128)
- Activation: ReLU
- Batch Normalization + Dropout (0.3)
- Output: 10 classes

### Experiment 2
- Input: Flatten (784)
- Hidden layers: 3 (512, 256, 128)
- Activation: ReLU
- Batch Normalization + Dropout
- Learning rate: 0.0001

---

## 🏋️ Training Details
- Optimizer: Adam
- Loss Function: CrossEntropyLoss
- Epochs: 10
- Metrics:
  - Accuracy
  - Loss

---

## 🔬 Experiments
- Experiment 1: LR = 0.001, 2 hidden layers
- Experiment 2: LR = 0.0001, 3 hidden layers

---

## 📈 Results
- Both models achieved ~88–89% test accuracy
- Experiment 2 showed slightly better generalization

---

## 📊 Visualizations
- Training vs Validation Loss curves
- Training vs Validation Accuracy curves
- Comparison between experiments

---

## 🧪 Regularization
- Dropout used to reduce overfitting
- Batch Normalization used to stabilize training

---

## 🚀 How to Run
```bash
pip install torch torchvision matplotlib pandas
