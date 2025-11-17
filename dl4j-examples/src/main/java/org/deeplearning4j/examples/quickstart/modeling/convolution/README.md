# Convolutional Neural Network (CNN) Examples – DeepLearning4J

This folder contains convolutional neural network (CNN) examples implemented using DeepLearning4J.

## 🧠 LeNetMNIST.java
Trains a LeNet-style CNN on the MNIST handwritten digit dataset.

### ✔ What this example demonstrates
- Loading the MNIST dataset
- Building a classic LeNet CNN architecture
- Training the network
- Evaluating accuracy

### ✔ Expected Accuracy
**98%–99%** after 1–2 epochs.

---

## 📦 How to Run

Build the project:

mvn clean package

Run the example:

mvn -q exec:java -Dexec.mainClass="org.deeplearning4j.examples.quickstart.modeling.convolution.LeNetMNIST"

Run the ReLU variant:

mvn -q exec:java -Dexec.mainClass="org.deeplearning4j.examples.quickstart.modeling.convolution.LeNetMNISTReLu"

---

## 🧱 LeNet Architecture Breakdown
- Convolution layer (20 filters)
- Subsampling (2×2)
- Convolution layer (50 filters)
- Subsampling
- Dense layer
- Output layer (Softmax, 10 classes)

---

## 📂 Other Files
| File | Description |
|------|-------------|
| **LeNetMNISTReLu.java** | LeNet variant with ReLU activation |
| **CenterLossLeNetMNIST.java** | LeNet with center loss |
| **CIFARClassifier.java** | CIFAR-10 image classifier |
| **Conv1DUCISequenceClassifier.java** | 1D CNN example for sequences |

---

## 🙌 Why This Documentation Helps
These CNN examples previously had no explanation, run instructions, or architecture summary.  
This README improves clarity for new users and first-time contributors.
