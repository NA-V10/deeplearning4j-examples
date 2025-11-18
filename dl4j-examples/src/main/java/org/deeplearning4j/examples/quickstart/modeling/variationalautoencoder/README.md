# Variational Autoencoder (VAE) Examples – DeepLearning4J

This folder contains two examples demonstrating how to use Variational Autoencoders (VAEs) in DeepLearning4J.  
VAEs are generative models that learn latent representations of data and can be used for visualization, sampling, and anomaly detection.

---

## 🧩 VaeMNIST2dPlots.java
Trains a VAE on the MNIST digit dataset and visualizes the **2-dimensional latent space**.

### What this example shows
- How to build a VAE in DL4J  
- Encoding MNIST images into a 2D latent space  
- Plotting how digits cluster in latent space  
- How VAEs learn smooth and continuous representations  

### Why it’s useful
A 2D latent space allows easy visualization of how the model separates digits.

---

## ⚠️ VaeMNISTAnomaly.java
Uses a trained VAE for **anomaly detection** on MNIST.

### Key Concepts
- VAEs reconstruct normal data well  
- They reconstruct anomalies poorly  
- Reconstruction error can be used as an anomaly score  

### What this example demonstrates
- Reconstructing MNIST digits  
- Computing reconstruction probability  
- Detecting out-of-distribution or corrupted samples  

---

## ✔ How to Run Any Example

mvn -q exec:java -Dexec.mainClass="org.deeplearning4j.examples.quickstart.modeling.variationalautoencoder.<ClassName>"


Example:



mvn -q exec:java -Dexec.mainClass="org.deeplearning4j.examples.quickstart.modeling.variationalautoencoder.VaeMNIST2dPlots"


---

## 🙌 Why This README Helps
The VAE folder previously had no documentation.  
This README explains:
- Purpose of each example  
- The ML concepts involved  
- How to run and understand the results  

This improves clarity for beginners working with generative models in DL4J.