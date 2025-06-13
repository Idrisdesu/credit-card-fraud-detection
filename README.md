# Credit Card Fraud Detection

This project explores credit card fraud detection using Machine Learning techniques. It compares the performance of a Logistic Regression model and an Artificial Neural Network (ANN) on an imbalanced transaction dataset.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Modeling & Results](#modeling--results)
- [Technologies Used](#technologies-used)
- [How to Run the Notebook](#how-to-run-the-notebook)

## Introduction

This notebook presents a practical approach to identifying fraudulent transactions. We evaluate the ability of Logistic Regression and an Artificial Neural Network (ANN) to handle a dataset where fraudulent cases are rare.

## Dataset

The dataset comes from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud). It contains anonymized transactions, with PCA-transformed features, as well as `Time` and `Amount`. The `Class` variable indicates whether a transaction is fraudulent (1) or not (0). It exhibits significant class imbalance.

## Data Preprocessing

Preprocessing steps include:
- **Normalization** of `Time` and `Amount` features (using `StandardScaler` or `RobustScaler`).
- **Class balancing** with `SMOTE` to address data imbalance.
- **Splitting** into training and test sets.

## Modeling & Results

We trained and evaluated two models:

1.  **Logistic Regression**
2.  **Artificial Neural Network (ANN)**

Models were primarily evaluated based on their accuracy and their ability to detect fraud (recall).

**Key results obtained:**
- **Logistic Regression:** 96.5% accuracy.
- **Artificial Neural Network (ANN):** 98.2% accuracy.

The Artificial Neural Network showed superior performance, particularly in correctly identifying fraudulent transactions, suggesting a better capture of non-linear relationships in the data.

## Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- TensorFlow, Keras
- Imbalanced-learn

## How to Run the Notebook

This notebook (`credit-card-fraud-detection.ipynb`) is **already available in this repository**.

To run it locally:

1.  Install dependencies:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn tensorflow keras imbalanced-learn jupyter
    ```
2.  Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
3.  Open the `credit-card-fraud-detection.ipynb` file.
