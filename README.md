# Fashion-MNIST Image Classification

A deep learning project that classifies clothing images from the Fashion-MNIST dataset using Logistic Regression and a Convolutional Neural Network (CNN). The project covers data exploration, preprocessing, model training, evaluation, and performance comparison.

## Project Overview

Fashion-MNIST contains 70,000 grayscale clothing images across 10 categories. Each image has a resolution of 28 × 28 pixels.

- Training set: 60,000 images
- Test set: 10,000 images
- Number of classes: 10

## Models

**Logistic Regression**
- Baseline classification model.
- Images are flattened into 784 features.
- Test accuracy: **84.31%**

**Convolutional Neural Network (CNN)**
- Uses convolution and pooling layers to learn image patterns.
- Includes dense layers and dropout.
- Test accuracy: **90.73%**

## Results

| Model | Test Accuracy | Training Time |
|---|---:|---:|
| Logistic Regression | 84.31% | 88.73 seconds |
| CNN | 90.73% | 359.16 seconds |

The CNN achieved a 6.42 percentage-point improvement in test accuracy over Logistic Regression, with a longer training time.

### Model Comparison

![Model Accuracy and Training Time Comparison](model_comparison.png)

## Key Findings

- CNN achieved higher test accuracy than Logistic Regression.
- Clothing categories with visually similar shapes were more challenging to classify.
- The Shirt category remained the most difficult class for the CNN.
- The confusion matrix helped identify common classification errors.

## Technologies Used

- Python
- TensorFlow / Keras
- Scikit-learn
- NumPy and Pandas
- Matplotlib and Seaborn
- Google Colab

## Repository Contents

- `fashion_mnist_deep_learning.ipynb` — Notebook containing the analysis, preprocessing, model training, and evaluation.
- `fashion_mnist_cnn.keras` — Saved trained CNN model.
- `model_comparison.csv` — Model accuracy and training-time results.
- `model_comparison.png` — Visual comparison of model performance.
- `class_names.json` — Class names used for clothing classification.

## How to Explore

Open the Jupyter Notebook in Google Colab to review the workflow and results. The saved CNN model can be loaded for further evaluation or inference.

## Future Improvements

- Improve classification of visually similar clothing categories.
- Experiment with CNN architectures and hyperparameters.
- Evaluate additional performance metrics.
- Build a simple interface for predicting clothing categories from images.
