# nn
# Handwritten Digit Recognition using MLP (MNIST)

## Project Description

This project implements a Multilayer Perceptron (MLP) neural network for handwritten digit recognition using the MNIST dataset.
The model classifies handwritten digits from 0 to 9.

---

## Dataset

MNIST Dataset
Dataset Source: TensorFlow / Keras built-in dataset

* Training Images: 60,000
* Testing Images: 10,000
* Image Size: 28 × 28 grayscale images

---

## Preprocessing Steps

* Image normalization
* One Hot Encoding for labels
* Train/Test split provided by MNIST dataset

---

## Model Architecture

The implemented MLP model contains:

* Flatten Layer
* Dense Hidden Layer (128 neurons)
* Batch Normalization
* Dropout Layer
* Dense Hidden Layer (64 neurons)
* Output Layer with Softmax activation

---

## Experiments

Two experiments were performed using different activation functions:

| Model   | Activation Function |
| ------- | ------------------- |
| Model A | ReLU                |
| Model B | Sigmoid             |

---

## Results

| Model             | Accuracy        | Loss        |
| ----------------- | --------------- | ----------- |
| Model A (ReLU)    | Higher Accuracy | Lower Loss  |
| Model B (Sigmoid) | Lower Accuracy  | Higher Loss |

ReLU achieved better performance and faster convergence compared to Sigmoid.

---

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib

---

## How to Run

Install required libraries:

```bash
pip install tensorflow numpy matplotlib
```

Run the project:

```bash
python main.py
```

---

## Output

The project generates:

* Training vs Validation Accuracy curves
* Training vs Validation Loss curves
* Model comparison table
* Digit prediction example
