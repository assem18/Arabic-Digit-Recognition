# Arabic Handwritten Digit Recognition using CNN and TensorFlow

## Overview

This project implements an Arabic Handwritten Digit Recognition System using Convolutional Neural Networks (CNNs) and the MAHDBase dataset.

The system is capable of:

* Loading and preprocessing Arabic handwritten digit images.
* Training a deep CNN classifier.
* Evaluating model performance using accuracy, loss curves, classification reports, and confusion matrices.
* Predicting handwritten digits from uploaded images.
* Recognizing multiple digits within a single image using contour-based segmentation.

---

## Dataset

The project uses the **MAHDBase (Modified Arabic Handwritten Digits Database)** dataset.

Dataset Statistics:

* Training Samples: 60,000 images
* Testing Samples: 10,000 images
* Classes: 10 digits (0–9)

---

## Technologies Used

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Matplotlib
* Scikit-Learn

---

## Model Architecture

The model is based on a Convolutional Neural Network (CNN):

Input (28×28×1)

↓

Conv2D (32 filters)

↓

Batch Normalization

↓

Max Pooling

↓

Conv2D (64 filters)

↓

Batch Normalization

↓

Max Pooling

↓

Conv2D (128 filters)

↓

Batch Normalization

↓

Flatten

↓

Dense (128)

↓

Dropout (0.4)

↓

Dense (10, Softmax)

---

## Results

### Final Performance

| Metric              | Value |
| ------------------- | ----- |
| Validation Accuracy | 99.5% |
| Training Accuracy   | 99.7% |
| Test Accuracy       | ~99%  |

The model demonstrates excellent generalization with minimal overfitting.

---

## Training Accuracy

![Accuracy Curve](results/accuracy_curve.png)

The training and validation accuracies converge smoothly and remain above 99%.

---

## Training Loss

![Loss Curve](results/loss_curve.png)

The loss decreases consistently throughout training, indicating stable learning behavior.

---

## Confusion Matrix

![Confusion Matrix](results/confusion_matrix.png)

The confusion matrix shows strong classification performance across all digit classes with very few misclassifications.

---

## Features

* Automatic image preprocessing
* CNN-based digit classification
* Multi-digit recognition
* Classification report generation
* Confusion matrix visualization
* Saved trained model (.keras)

---

## Repository Structure

```text
Arabic_Digit_Recognition_System/

│
├── Arabic_Digit_Recognition_System.ipynb
├── best_arabic_digit_model.keras
├── requirements.txt
│
├── results/
│   ├── accuracy_curve.png
│   ├── loss_curve.png
│   └── confusion_matrix.png
│
└── README.md
```

## Future Improvements

* Arabic handwritten word recognition
* Real-time webcam digit recognition
* Flask web deployment
* Mobile deployment using TensorFlow Lite
* Transformer-based image classification models

---

## Author

Assem Aldurini

Computer Science (Artificial Intelligence)

Zewail City University
