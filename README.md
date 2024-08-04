# Estimation of Obesity Levels Based on Eating Habits and Physical Condition

## Introduction

Welcome to this repository where we analyze the **Estimation of Obesity Levels** dataset from the UC Irvine Machine Learning Repository. This dataset provides insights into how eating habits and physical conditions correlate with obesity levels, with the ultimate goal of building effective predictive models.

## Repository Structure

This repository contains:

- **`predicting-obesity-with-random-forests.ipynb`**: The Jupyter notebook with the complete analysis, including data preprocessing, model training, and evaluation.
- **`data/`**: Folder containing the dataset files:
  - **`original_data.csv`**: Raw data with some random NULL values.
  - **`data_ready.csv`**: A cleaned and imputed subset of 1,000 samples for model training and testing. Columns 'gender' and 'Weight' were removed to enhance model performance and avoid collinearity.
  - **`test_later.csv`**: Additional data for final model evaluation.

## Model Training and Evaluation

We employed a Random Forest Classifier, which was trained and tuned using cross-validation. Key results include:

### On `data_ready.csv`:

- **Accuracy**: 0.78
- **Recall for Class 1 (Obesity)**: 0.87

### On `test_later.csv`:

- **Accuracy**: 0.79
- **Recall for Class 1 (Obesity)**: 0.81

The recall for identifying obesity, our primary objective, demonstrates the model’s effectiveness in detecting individuals with obesity. The notebook details the model development process, including data preprocessing, feature engineering, and hyperparameter tuning.

## Explore Further

- **Kaggle Notebook**: Dive deeper into the analysis and code by visiting the Kaggle notebook [here](https://www.kaggle.com/code/jbasurtod/predicting-obesity-with-random-forests).
- **Live Model**: Experience the model in action on the Streamlit app [here](https://obesitypred.streamlit.app/).

## Getting Started

To replicate the analysis, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/obesity-estimation.git

2. Navigate to the project directory:
   ```bash
   cd predicting_obestiy_random_forests


3. Install Jupyter if needed
   ```bash
   pip install jupyter


4. Open the Notebook in Jupyter:
   ```bash
   jupyter notebook predicting-obesity-with-random-forests.ipynb
