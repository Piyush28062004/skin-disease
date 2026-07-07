# Skin Disease Classification using Deep Learning

A deep learning project for automated skin disease classification using Convolutional Neural Networks (CNNs) and TensorFlow. This project implements a complete image classification pipeline, including dataset preprocessing, class imbalance handling, data augmentation, model training, and evaluation.

---

## Project Overview

Skin diseases are among the most common health conditions worldwide. Manual diagnosis requires expert dermatologists and can be time-consuming. This project aims to assist the diagnostic process by classifying skin disease images using a custom CNN model.

The pipeline includes:

- Dataset preprocessing
- Corrupt image removal
- Automatic class detection
- Class imbalance analysis
- Stratified dataset splitting
- Data augmentation
- CNN-based image classification
- Early stopping and model checkpointing

---

## Features

- Automatic dataset organization
- Removal of corrupted images
- Stratified Train/Validation/Test split
- Efficient TensorFlow `tf.data` pipeline
- Data augmentation
- Class weight computation for imbalanced datasets
- Custom CNN architecture
- Early Stopping
- Model Checkpointing
- Visualization of dataset distribution

---

## Dataset

The dataset consists of dermoscopic skin disease images organized into class-wise folders.

Since the dataset exceeds GitHub's file size limit, it is not included in this repository.

Download the dataset from:

> *(Add Google Drive or Kaggle link here.)*

---

## Project Workflow

```
Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Class Detection
     │
     ▼
Dataset Analysis
     │
     ▼
Train / Validation / Test Split
     │
     ▼
Data Augmentation
     │
     ▼
Class Weight Computation
     │
     ▼
CNN Model
     │
     ▼
Training
     │
     ▼
Evaluation
```

---

## Model Architecture

The project uses a custom Convolutional Neural Network consisting of:

- Convolution Layers
- MaxPooling Layers
- ReLU Activation
- Dense Layers
- Softmax Output Layer

Input image size:

```
224 × 224 × 3
```

Optimizer:

```
Adam
```

Learning Rate:

```
0.0001
```

Loss Function:

```
Sparse Categorical Crossentropy
```

---

## Data Preprocessing

The preprocessing pipeline includes:

- Automatic class detection
- Corrupt image removal
- Image resizing
- Normalization
- TensorFlow Dataset API
- Batch processing
- Prefetching

---

## Data Augmentation

Training images are augmented using:

- Horizontal Flip
- Rotation
- Zoom
- Translation

This improves generalization and reduces overfitting.

---

## Handling Class Imbalance

The project computes class weights using Scikit-learn's `compute_class_weight()` function and applies them during training to improve performance on minority classes.

---

## Training

Training configuration:

- TensorFlow / Keras
- Adam Optimizer
- EarlyStopping
- ModelCheckpoint
- Batch Size: 16
- Image Size: 224 × 224
- Epochs: 20

---

## Repository Structure

```
.
├── notebooks/
├── models/
├── images/
├── dataset/
├── README.md
├── requirements.txt
└── LICENSE
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/skin-disease-classification.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
archive1_skin_disease.ipynb
```

---

## Results

After training, the model can classify skin disease images using the learned CNN.

*(Add your final accuracy, precision, recall, and F1-score here once available.)*

---

## Future Improvements

- Transfer Learning using EfficientNetB4
- DenseNet121
- MobileNetV3
- Grad-CAM visualization
- Hyperparameter optimization
- Model deployment using Flask or FastAPI
- Docker support

---

## Author

**Piyush**

Final Year B.Tech Student

---

## License

This project is released under the MIT License.
