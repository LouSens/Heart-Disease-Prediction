# Heart Disease Prediction using Random Forest

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-orange)
![pandas](https://img.shields.io/badge/pandas-1.3%2B-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

A comprehensive machine learning project that predicts the presence of heart disease using the Random Forest algorithm.

## 📋 Overview

This project analyzes a heart disease dataset containing various patient attributes and builds a Random Forest classifier to predict whether a patient has heart disease. The implementation follows industry best practices with a complete machine learning pipeline including exploratory data analysis, preprocessing, model building, hyperparameter tuning, and evaluation.

## 🔍 Dataset

The dataset contains 999 records with 13 features and 1 target variable:

- **age**: Patient age in years.
- **sex**: Gender (1 = male, 0 = female).
- **cp**: Chest pain type (0-3).
- **trestbps**: Resting blood pressure (mmHg).
- **chol**: Serum cholesterol (mg/dl).
- **fbs**: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false).
- **restecg**: Resting ECG results (0-2).
- **thalach**: Maximum heart rate achieved (bpm).
- **exang**: Exercise-induced angina (1 = yes, 0 = no).
- **oldpeak**: ST depression induced by exercise.
- **slope**: Slope of peak exercise ST segment (0-2).
- **ca**: Number of major vessels (0-4).
- **thal**: Thalassemia indicator (0-3).
- **target**: Heart disease presence (1 = yes, 0 = no).

## 🏗️ Project Structure

heart-disease-prediction/
````
│
├── heart.csv                          # Dataset file
├── Heart_Disease_Prediction.ipynb     # Main script
````

## 🚀 Features

- **Random Forest Classifier**: Ensemble of 100 decision trees for accurate predictions.
- **Data Preprocessing**: Splits data into 80% training and 20% testing sets.
- **Model Training**: Trains on preprocessed data with reproducible results (random_state=42).
- **Prediction Evaluation**: Provides accuracy (0.99), classification report, and confusion matrix.
- **Feature Importance**: Visualizes key predictors like thalach and oldpeak.
- **Visualizations**: Includes target distribution, correlation heatmap, and feature importance plots.



## 📊 Results

The Random Forest model achieves strong performance in predicting heart disease with the accuracy of 99%.

Key findings from the analysis:
- Chest pain type (cp), maximum heart rate (thalach), and number of major vessels (ca) are the most important predictors
- There's a strong negative correlation between thalach (maximum heart rate) and heart disease
- Men are more likely to have heart disease in this dataset

## 📦 Requirements

- Python 3.8+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.
