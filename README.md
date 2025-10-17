# Perceptron Implementation using Python

## Overview

This project demonstrates the implementation of the **Perceptron algorithm** for simple logical functions such as **AND** and **OR** using Python.  
The goal is to understand the fundamentals of **linear classification**, **activation functions**, and **decision boundaries** in neural networks.

The perceptron model was built and trained using the `MLPClassifier` from the **scikit-learn** library.  
The notebook also visualizes how weights and decision regions evolve during learning.

---

## Table of Contents
- [Concept](#concept)
- [Methodology](#methodology)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Usage](#usage)

---

## Concept

The **Perceptron** is the simplest form of a neural network — a single neuron that performs binary classification.  
It combines inputs using weighted sums and passes them through an activation function to produce an output.

Mathematically:
```
y = f(w₁x₁ + w₂x₂ + ... + b)
```
where **f** is the activation function (e.g., step or sigmoid).

This lab implements perceptrons for:
- **AND Function**
- **OR Function**

and analyzes whether they can learn the expected truth table through supervised training.

---

## Methodology

1. **Dataset Preparation**
   - Constructed truth tables for logical AND and OR gates.
   - Encoded inputs and expected outputs.

2. **Model Initialization**
   - Used `MLPClassifier` from `scikit-learn` with a single hidden layer.
   - Set activation to `'logistic'` for sigmoid-like behavior.

3. **Training Process**
   - Fitted the model on each logical dataset.
   - Adjusted learning rate and iterations for convergence.

4. **Evaluation**
   - Printed predicted vs actual outputs.
   - Visualized decision regions and weight effects.

---

## Results

### AND Gate
| Input (x1, x2) | Expected | Predicted |
|----------------|-----------|------------|
| (0, 0) | 0 | 0 |
| (0, 1) | 0 | 0 |
| (1, 0) | 0 | 0 |
| (1, 1) | 1 | 1 |

✅ The perceptron successfully learned the AND function.

### OR Gate
| Input (x1, x2) | Expected | Predicted |
|----------------|-----------|------------|
| (0, 0) | 0 | 0 |
| (0, 1) | 1 | 1 |
| (1, 0) | 1 | 1 |
| (1, 1) | 1 | 1 |

✅ The perceptron successfully learned the OR function.

---

## Technologies Used

- **Language:** Python 3.9+  
- **Libraries:**
  - NumPy
  - Scikit-learn
  - Matplotlib
- **Tools:**
  - Jupyter Notebook

---

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/mehmet-akif/perceptron-python-implementation.git
   cd perceptron-python-implementation
   ```

2. Install dependencies:
   ```bash
   pip install numpy matplotlib scikit-learn
   ```

3. Launch the notebook:
   ```bash
   jupyter notebook Lab-6-AKIF_SIPAHI.ipynb
   ```

4. Run all cells to reproduce:
   - AND and OR gate perceptron models  
   - Decision region visualization  



---

## License

© 2025 Mehmet Akif Sipahi. All rights reserved.  
This project is shared for educational and portfolio demonstration purposes only.  
Reproduction, redistribution, or submission of this material for academic credit is strictly prohibited.
