# Unsupervised Learning Examples – Autoencoder (DeepLearning4J)

This folder contains unsupervised learning examples implemented using DeepLearning4J.  
The primary example in this directory demonstrates how to train an autoencoder on MNIST digits to perform dimensionality reduction and reconstruction.

---

## 🧠 MNISTAutoencoder.java

A simple autoencoder trained on the MNIST dataset (28×28 grayscale digit images).  
Autoencoders learn to compress input data into a lower-dimensional representation and then reconstruct it.

### What this example shows
- How autoencoders work
- How to compress images into a bottleneck latent space
- How to reconstruct input images
- How unsupervised neural networks are trained

### Key Concepts
- **Encoder:** Compresses image → latent representation  
- **Decoder:** Reconstructs latent representation → image  
- **Loss Function:** Measures reconstruction quality  

### Expected Behavior
The autoencoder gradually learns to:
- Rebuild digit outlines
- Capture key features
- Reduce noise

This is not a classifier — it learns **patterns** without labels.

---

## ✔ How to Run

mvn -q exec:java -Dexec.mainClass="org.deeplearning4j.examples.quickstart.modeling.feedforward.unsupervised.MNISTAutoencoder"


---

## 🙌 Why This README Helps
The unsupervised folder previously had no explanation, run instructions, or conceptual overview.  
This documentation improves clarity and helps beginners understand autoencoders and unsupervised learning techniques in DL4J.