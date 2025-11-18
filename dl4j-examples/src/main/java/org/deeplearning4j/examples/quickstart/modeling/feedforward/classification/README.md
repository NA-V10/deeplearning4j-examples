# Feedforward Neural Network Classification Examples – DeepLearning4J

This folder contains several feedforward neural network (MLP) classification examples using DeepLearning4J.  
They demonstrate how to train neural networks on classic datasets such as MNIST, Iris, XOR, and synthetic datasets.

---

## 🧠 MNISTSingleLayer.java
A simple single-hidden-layer MLP for MNIST digit classification.

### What this example shows
- Loading MNIST data
- Building a minimal feedforward model
- Backpropagation training
- Evaluating test accuracy

---

## 🧠 MNISTDoubleLayer.java
A deeper MLP with two hidden layers for MNIST.

### Why it's useful
- Shows the impact of depth on accuracy
- Good introduction to multi-layer feedforward networks

---

## 🌸 IrisClassifier.java
A classifier for the Iris flower dataset.

### What you learn
- Basic classification with a very small dataset
- How to use evaluation metrics
- Simple preprocessing

---

## 🧪 ModelXOR.java
A classic MLP solving the XOR problem.

### Why XOR?
- Not linearly separable
- Demonstrates why deep networks are needed

---

## 🌙 MoonClassifier.java
Binary classification on a synthetic two-moon dataset.

### Learnings
- Handling noisy 2D datasets
- Visualizing classification boundaries

---

## 🪐 SaturnClassifier.java
Classification of Saturn (concentric circles) synthetic dataset.

### Shows
- Decision boundaries
- How MLPs learn non-linear patterns

---

## ✔ How to Run Any Example

Use the following command template:


mvn -q exec:java -Dexec.mainClass="org.deeplearning4j.examples.quickstart.modeling.feedforward.classification.<ClassName>"


Example:



mvn -q exec:java -Dexec.mainClass="org.deeplearning4j.examples.quickstart.modeling.feedforward.classification.MNISTSingleLayer"


---

## 🙌 Why This README Helps
These classification examples previously had no documentation.  
This README improves clarity, explains datasets, and helps beginners understand each example.