This repository contains the code used in my Master's dissertation titled "**Using Machine Learning and Deep Learning Methods in Predicting Patients with Diabetes**." The project explores various classification algorithms, resampling techniques, unbiased data approaches, and the application of Self-Normalizing Neural Networks (SNN) for diabetes prediction.

## Project Overview

- **Title**: Using Machine Learning and Deep Learning Methods in Predicting Patients with Diabetes
- **Objective**: Implement various machine learning and deep learning models to predict diabetes and assess their performance. The project also focuses on improving model performance with unbiased data and resampling techniques to address class imbalance.
- **Models Used**: Logistic Regression, Random Forest, SVM, Gradient Boosting, XGBoost, Neural Networks, Self-Normalizing Neural Networks (SNN).
- **Techniques Applied**: 
  - **Resampling**: Techniques like oversampling the minority class (e.g., SMOTE) and undersampling the majority class to balance the dataset and mitigate bias.
  - **Unbiased Data**: Ensuring that the model is trained on a balanced and representative dataset to reduce bias and improve generalizability.
  - **Self-Normalizing Neural Networks (SNN)**: Applied to enhance the deep learning model's performance, especially in handling complex, high-dimensional data.

- **Tools & Libraries**: Python, Scikit-learn, TensorFlow, SHAP, Pandas, Numpy, Matplotlib

## Repository Contents

- `src/`: Contains all Python scripts and Jupyter notebooks for:
  - **Data Preprocessing**: Scripts for cleaning, normalizing, and preparing the data.
  - **Resampling**: Code for applying techniques like SMOTE and undersampling.
  - **Model Training & Evaluation**: Training various machine learning models and deep learning architectures, including SNN.
  - **Model Interpretability**: Using SHAP for explaining model predictions.

- `data/`: Sample dataset (or a link to the data source if sensitive).
- `results/`: Outputs, figures, and performance metrics from different models and techniques.
- `requirements.txt`: Python dependencies for the project.

## Key Concepts

### Resampling Techniques
Class imbalance can lead to biased predictions, where the model favors the majority class. To address this, we applied resampling methods:
- **Oversampling the minority class** using SMOTE (Synthetic Minority Over-sampling Technique).
- **Undersampling the majority class** to ensure balanced training data.

### Unbiased Data
The goal was to create models that could generalize well without bias toward any particular class. Ensuring balanced data through resampling techniques helped mitigate biases in the predictions.

### Self-Normalizing Neural Networks (SNN)
SNN is a specialized neural network architecture that maintains a stable distribution of activations during the training process. This allows the network to self-normalize, avoiding the need for explicit normalization layers like batch normalization, which can be particularly useful when working with complex datasets like those used for diabetes prediction.

## Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/repository-name.git
