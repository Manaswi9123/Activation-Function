# Activation-Function
# ⚡ Neural Network Activation Functions

This repository provides a mathematical and programmatic breakdown of **Activation Functions**, the "gates" of a neural network that determine whether a neuron should fire and pass information forward.

---

## 🛠️ The Math Stack
* **Language:** Python
* **Library:** `math` (Native Python library for transcendental functions)
* **Concepts:** Non-linearity, Probability mapping, and Gradient management.

---

## 🧠 Functions Implemented

### 1. Sigmoid Function
Maps any real value into a range between **0 and 1**. 
* **Use Case:** Output layers for binary classification and modeling probability.
* **Equation:** $\sigma(x) = \frac{1}{1 + e^{-x}}$

### 2. Tanh (Hyperbolic Tangent)
Maps values into a range between **-1 and 1**.
* **Use Case:** Generally preferred over Sigmoid in hidden layers as it centers the data around zero, making the learning process faster for the next layer.

### 3. ReLU (Rectified Linear Unit)
Outputs the input directly if it is positive; otherwise, it outputs zero.
* **Use Case:** The most common activation function for hidden layers in modern deep learning due to its simplicity and ability to reduce the "Vanishing Gradient" problem.
* **Equation:** $f(x) = \max(0, x)$

### 4. Leaky ReLU
A variation of ReLU that allows a small, non-zero gradient when the input is negative.
* **Use Case:** Designed to solve the "Dying ReLU" problem by ensuring neurons never completely stop learning.
* **Equation:** $f(x) = \max(0.1x, x)$

---

## 📈 Why are these important?
Without these functions, a Neural Network would just be a giant **Linear Regression** model. Activation functions introduce **non-linearity**, allowing the network to learn complex patterns like recognizing faces, understanding speech, or driving cars.



---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Manaswi9123/Python-DataScience-Fundamentals.git](https://github.com/Manaswi9123/Python-DataScience-Fundamentals.git)

2. **Execute:** Open ActivationFunction.ipynb in any Jupyter environment.

3. **Experiment:** Pass extreme values (like 100 or -100) into the functions to see how they "squash" or "clip" the results.
