[mnist_ann_project_readme_and_submission_files.md](https://github.com/user-attachments/files/27861339/mnist_ann_project_readme_and_submission_files.md)
# MNIST Handwritten Digit Recognition using Artificial Neural Networks (ANN)

## Project Description

This project implements a Multilayer Perceptron (MLP) model for handwritten digit recognition using the MNIST dataset.

The project was developed as part of the Neural Networks course requirements.

Three different experiments were conducted using different activation functions:

1. ReLU Activation Function
2. Sigmoid Activation Function
3. Tanh Activation Function

The purpose of the experiments is to compare the performance of different activation functions in image classification tasks.

---

# Dataset

Dataset Used:
- MNIST Handwritten Digits Dataset

Dataset Link:
- https://www.tensorflow.org/datasets/catalog/mnist

Dataset Description:
- 60,000 training images
- 10,000 testing images
- Image size: 28 × 28 pixels
- Classes: Digits from 0 to 9

---

# Data Preprocessing

The following preprocessing steps were applied:

- Normalization of pixel values by dividing by 255
- Splitting dataset into training and testing sets
- Checking for missing values

No missing values were found in the dataset.

---

# Model Architecture

The implemented model is a Multilayer Perceptron (MLP) consisting of:

- Input Layer
- Hidden Layer
- Output Layer

Output layer uses the Softmax activation function for multiclass classification.

Loss Function:
- Sparse Categorical Crossentropy

Optimizer:
- Adam Optimizer

Evaluation Metric:
- Accuracy

---

# Experiments

## Experiment 1 — ReLU Activation

Architecture:
- Flatten Layer
- Dense Layer (128 neurons, ReLU)
- Output Layer (10 neurons, Softmax)

---

## Experiment 2 — Sigmoid Activation

Architecture:
- Flatten Layer
- Dense Layer (128 neurons, Sigmoid)
- Output Layer (10 neurons, Softmax)

---

## Experiment 3 — Tanh Activation

Architecture:
- Flatten Layer
- Dense Layer (128 neurons, Tanh)
- Output Layer (10 neurons, Softmax)

---

# Training Details

The models were trained using:

- Epochs: 20
- Batch Size: 32
- Validation Split: 20%
- EarlyStopping callback to prevent overfitting

---

# Results

| Experiment | Activation Function | Accuracy | Loss |
|---|---|---|---|
| Experiment 1 | ReLU | 0.9746 | 0.0814 |
| Experiment 2 | Sigmoid |0.9283 | 0.2496 |
| Experiment 3 | Tanh | 0.9456 |0.1831 |

---

# Visualizations

The following graphs were generated for each experiment:

- Training vs Validation Accuracy
- Training vs Validation Loss

These visualizations help analyze model performance and detect overfitting.

---

# Libraries Used

- TensorFlow
- NumPy
- Matplotlib

---

# How to Run the Project

1. Install required libraries:

```bash
pip install tensorflow numpy matplotlib
```

2. Run the Python file:

```bash
python ann_project.py
```

---

# Project Structure

```text
ANN_Project/
│
├── ann_project.py
├── README.md
├── results/
│   ├── accuracy_graphs.png
│   ├── loss_graphs.png
│
└── requirements.txt
```

---

# Conclusion

The experiments demonstrate that activation functions significantly affect neural network performance.

Among the tested activation functions:
- ReLU generally provides the best performance and fastest convergence.
- Sigmoid performs adequately but may suffer from vanishing gradients.
- Tanh performs better than Sigmoid in some cases because its output is centered around zero.

---

# Author

Student Name: Rola Hany Tharwat

Course: Neural Networks

