# Recurrent Neural Network (RNN) Examples – DeepLearning4J

This folder contains simple recurrent neural network (RNN) examples using LSTM and embedding layers.  
These examples demonstrate how to work with sequential data such as signals, sequences, and text-like inputs.

---

## 🔁 MemorizeSequence.java
A minimal RNN example where the network learns to memorize and reproduce a fixed sequence.

### What this example teaches
- How RNNs store information across time steps  
- How backpropagation-through-time works  
- How sequence learning differs from feedforward networks  

### Expected Behavior
The network eventually outputs the same sequence it was trained on.

---

## 🔡 RNNEmbedding.java
Demonstrates the use of an **EmbeddingLayer** followed by RNN layers.

### Key Concepts
- Turning integer-encoded inputs into dense vectors  
- Word/token embedding  
- Passing embedded sequences into RNN layers  

This is a useful template for NLP-style models.

---

## 📊 UCISequenceClassification.java
Sequence classification on a dataset from the UCI machine learning repository.

### What this example shows
- Loading sequential datasets  
- Recurrent classification (predict a label for a whole sequence)  
- Time-series preprocessing and normalization  

---

## ✔ How to Run Any Example

Use the following command:

mvn -q exec:java -Dexec.mainClass="org.deeplearning4j.examples.quickstart.modeling.recurrent.<ClassName>"


Example:



mvn -q exec:java -Dexec.mainClass="org.deeplearning4j.examples.quickstart.modeling.recurrent.MemorizeSequence"


---

## 🙌 Why This README Helps

This folder previously had no documentation.  
This README explains:
- What each RNN example does  
- What concepts it teaches  
- How to run each file  

This improves clarity for beginners working with sequential models in DL4J.