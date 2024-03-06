# README for CCFraudML (Credit Card Fraud Detection Model)

## Introduction
Credit card fraud detection using Scikit-Learn and Snap ML. This README provides an overview of a machine learning model designed to detect credit card fraud using Python and Snap ML. The model utilizes supervised learning techniques and is implemented using the `snapml` library for efficient training and inference.

## Setup
Before running the code, ensure you have the required libraries installed. You can install them using pip:
`!pip install snapml`


## Dataset
The dataset used for training and evaluation is available at the following URL:
[Credit Card Fraud Dataset](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-ML0101EN-SkillsNetwork/labs/Module%203/data/creditcard.csv)

## Code Overview
1. **Import Libraries**: Install necessary packages and import required libraries.
2. **Data Preprocessing**: Read the dataset, inflate it to replicate actual size, and perform data normalization.
3. **Train/Test Split**: Split the dataset into training and testing sets.
4. **Build Decision Tree Classifier (DTC)**: Train a DTC model using both Scikit-Learn and Snap ML, compare training times and ROC-AUC scores.
5. **Build Support Vector Machine (SVM)**: Train a SVM model using both Scikit-Learn and Snap ML, compare training times and ROC-AUC scores.
6. **Model Evaluation**: Evaluate the quality of SVM models using the hinge loss metric.

## Results
- **Decision Tree Classifier (DTC)**:
  - Snap ML vs. Scikit-Learn speedup: 7.62x
  - Scikit-Learn ROC-AUC score: 0.966
  - Snap ML ROC-AUC score: 0.966

- **Support Vector Machine (SVM)**:
  - Snap ML vs. Scikit-Learn speedup: 4.68x
  - Scikit-Learn ROC-AUC score: 0.984
  - Snap ML ROC-AUC score: 0.985
  - Hinge Loss (Snap ML): 0.228
  - Hinge Loss (Scikit-Learn): 0.234

## Conclusion
The Snap ML library demonstrates significant speedup in training time compared to Scikit-Learn while maintaining comparable model performance metrics, making it a valuable tool for large-scale machine learning tasks.
