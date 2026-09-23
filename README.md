# Handwritten Digit Recognition using Feedforward Neural Network (MNIST)

This project implements a **Feedforward Neural Network (FNN)** — also known as a **Multilayer Perceptron (MLP)** — to classify handwritten digits from the **MNIST dataset** using **TensorFlow/Keras**.

---

## Project Overview

- The model learns to recognize digits **0–9** from 28×28 grayscale images.  
- It uses two hidden layers with ReLU activation and a softmax output layer.  
- The network is trained using **Stochastic Gradient Descent (SGD)** optimizer and **categorical cross-entropy** loss.  
- Performance is evaluated on the MNIST test set and visualized with prediction plots.

---

## Model Architecture

| Layer | Type | Units | Activation |
|-------|------|--------|-------------|
| 1 | Dense (Hidden) | 128 | ReLU |
| 2 | Dense (Hidden) | 128 | ReLU |
| 3 | Dense (Output) | 10 | Softmax |

---

## Key Steps
1. **Data Loading** – MNIST digits from `keras.datasets.mnist`.  
2. **Preprocessing** – Flatten 28×28 images into 784-length vectors and normalize pixels (0–1).  
3. **Encoding Labels** – One-hot encoding using `to_categorical()`.  
4. **Model Building** – `Sequential` model with 3 dense layers.  
5. **Training** – Optimizer = `SGD`, Loss = `categorical_crossentropy`, Metric = `accuracy`.  
6. **Evaluation & Visualization** – Test accuracy and grid of predictions with color-coded results.

---

## Example Results
Typical performance:
- **Training accuracy:** ~97–99%  
- **Test accuracy:** ~93–96%

---

## Requirements
tensorflow
numpy
matplotlib
(One can install them with `pip install -r requirements.txt`)

---

## Visualization
The notebook displays a 5×5 grid of test digits,  
with green labels for **correct** and red labels for **incorrect** predictions.

---

## Files
- `mnist.ipynb` – main notebook with full code and outputs  
- `README.md` – project description (this file)  
- `requirements.txt` *(optional)* – package list  

---

## Acknowledgment
Dataset: [MNIST Handwritten Digits](http://yann.lecun.com/exdb/mnist/)  
Framework: [TensorFlow / Keras](https://www.tensorflow.org/)

---

## How to Run
1. Clone this repo  
2. Install dependencies  
3. Run the notebook in Jupyter or Google Colab  




