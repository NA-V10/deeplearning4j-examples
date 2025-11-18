# ND4J NDArray Examples

This module contains simple examples that demonstrate how to use **ND4J**  
(N-dimensional arrays for Java) — the core numerical computing library behind Deeplearning4j.

ND4J provides fast tensor operations similar to NumPy, backed by optimized BLAS  
implementations.

These examples help new users understand:

- What an `INDArray` is  
- How to create arrays  
- How to perform basic math  
- How to reshape, slice, and combine arrays  
- How to run the examples using Maven

---

## 📌 What is an NDArray?

An **NDArray** (N-dimensional array) is ND4J’s fundamental data structure.  
It represents:

- Scalars (0D)
- Vectors (1D)
- Matrices (2D)
- Higher dimensional tensors (3D, 4D, …)

ND4J operations are *vectorized* and run efficiently on CPU or GPU (via CUDA backend).

Example:

```java
INDArray arr = Nd4j.create(new float[]{1, 2, 3});
System.out.println(arr);   // [1.00, 2.00, 3.00]
📘 Basic NDArray Operations
Create Arrays
java

INDArray zeros = Nd4j.zeros(3, 3);
INDArray ones = Nd4j.ones(2, 2);
INDArray random = Nd4j.rand(1, 5);
INDArray arange = Nd4j.arange(1, 10);
Math Operations
java

INDArray a = Nd4j.create(new float[]{1, 2, 3});
INDArray b = Nd4j.create(new float[]{4, 5, 6});

System.out.println(a.add(b));       // elementwise add  
System.out.println(a.mul(b));       // elementwise multiply
System.out.println(a.mmul(b.T()));  // matrix multiplication
Reshape and Shape Ops
java
Copy code
INDArray m = Nd4j.linspace(1, 9, 9).reshape(3, 3);
System.out.println(m);

System.out.println(m.transpose());
System.out.println(m.permute(1, 0));
▶️ How to Run These Examples
Make sure you have:

Java 8 or later

Maven installed

Then run:


mvn -q exec:java -Dexec.mainClass="org.nd4j.examples.quickstart.BasicNDArrayExample"
Or run any other example under:



src/main/java/org/nd4j/examples/
Example:


mvn -q exec:java -Dexec.mainClass="org.nd4j.examples.advanced.SlicingExample"
📤 Expected Output (Sample)
Running a basic NDArray creation example:


Copy code
Zeros array:
[[0.00, 0.00, 0.00],
 [0.00, 0.00, 0.00],
 [0.00, 0.00, 0.00]]

Random array:
[0.42, 0.91, 0.12, 0.55, 0.33]

Vector add:
[5.00, 7.00, 9.00]
📁 Project Structure

nd4j-ndarray-examples/
 ├── src/
 │   └── main/java/org/nd4j/examples/
 │        ├── advanced/
 │        ├── quickstart/
 │        ├── utils/
 │        └── resources/
 ├── pom.xml
 └── README.md
📄 License
This project is part of the Eclipse Deeplearning4j examples collection
and is licensed under the Apache License 2.0.

Happy coding with ND4J tensors! 🚀

