# Fashion-MNIST Image Classification

A deep learning project that classifies clothing images from the Fashion-MNIST dataset using Logistic Regression and a Convolutional Neural Network (CNN). The project covers data exploration, preprocessing, model training, evaluation, and performance comparison.

## Project Overview

Fashion-MNIST contains 70,000 grayscale clothing images across 10 categories, with each image measuring 28 × 28 pixels.

- **Training set:** 60,000 images
- **Test set:** 10,000 images
- **Number of classes:** 10

## Models

### Logistic Regression

A baseline machine learning model used to classify flattened image data.

- **Input features:** 784 per image
- **Test accuracy:** 84.31%
- **Training time:** 88.73 seconds

### Convolutional Neural Network (CNN)

A deep learning model that uses convolutional and pooling layers to learn visual patterns in clothing images.

- **Architecture:** Convolutional, max pooling, dense, and dropout layers
- **Test accuracy:** 90.73%
- **Training time:** 359.16 seconds

## Results

| Model | Test Accuracy | Training Time |
|---|---:|---:|
| Logistic Regression | 84.31% | 88.73 seconds |
| CNN | 90.73% | 359.16 seconds |

The CNN improved test accuracy by **6.42 percentage points** compared with Logistic Regression, although it required more training time.

## Model Comparison

The following chart compares the test accuracy and training time of both models.

![Model Comparison](model_comparison.png)

## CNN Confusion Matrix

The confusion matrix shows the CNN's classification performance across all 10 clothing categories. Values along the diagonal represent correct predictions, while off-diagonal values indicate misclassified images.

![CNN Confusion Matrix](cnn-confusion-matrix.png)

The CNN performed particularly well on Trousers, Sandals, Bags, and Sneakers. Shirts were more challenging to classify, with errors involving visually similar clothing categories.

## Key Findings

- CNN achieved higher test accuracy than Logistic Regression.
- Visually similar clothing categories were more difficult to distinguish.
- Shirt was the most challenging class for the CNN.
- The confusion matrix helped identify common classification errors.

## Technologies Used

- Python
- TensorFlow / Keras
- Scikit-learn
- NumPy and Pandas
- Matplotlib and Seaborn
- Google Colab

## Repository Contents

- `fashion_mnist_deep_learning.ipynb` — Notebook containing data exploration, preprocessing, model training, and evaluation.
- `fashion_mnist_cnn.keras` — Saved trained CNN model.
- `model_comparison.csv` — Model performance and training-time results.
- `model_comparison.png` — Visual comparison of model performance.
- `cnn-confusion-matrix.png` — CNN classification confusion matrix.
- `class_names.json` — Clothing class labels.

## Explore the Notebook

Explore the complete workflow, code, and results in Google Colab.

[Open Fashion-MNIST Notebook](https://colab.research.google.com/drive/1UOb0S2dyF9T_mSoJr1vCIsCbMDonoXyN?usp=sharing)

## How to Explore

1. Open the notebook in Google Colab.
2. Review the dataset exploration and preprocessing steps.
3. Examine the Logistic Regression and CNN training processes.
4. Compare model accuracy and training time.
5. Review the confusion matrix to understand classification errors.

## Future Improvements

- Improve classification of visually similar clothing categories.
- Experiment with CNN architectures and hyperparameters.
- Evaluate additional classification metrics.
- Develop a simple interface for predicting clothing categories from images.

## Project Information

- **Project:** Fashion-MNIST Image Classification
- **Category:** Machine Learning and Deep Learning
- **Task:** Multiclass Image Classification
- **Environment:** Google Colab

