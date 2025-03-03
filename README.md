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

- **age**: Age in years
- **sex**: Sex (1 = male, 0 = female)
- **cp**: Chest pain type (0-3)
- **trestbps**: Resting blood pressure (in mm Hg)
- **chol**: Serum cholesterol (in mg/dl)
- **fbs**: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
- **restecg**: Resting electrocardiographic results (0-2)
- **thalach**: Maximum heart rate achieved
- **exang**: Exercise induced angina (1 = yes, 0 = no)
- **oldpeak**: ST depression induced by exercise relative to rest
- **slope**: Slope of the peak exercise ST segment (0-2)
- **ca**: Number of major vessels colored by fluoroscopy (0-4)
- **thal**: Thalassemia (0-3)
- **target**: Heart disease diagnosis (1 = disease, 0 = no disease)

## 🏗️ Project Structure

```
heart-disease-prediction/
│
├── heart.csv                       # Dataset file
├── heart_disease_prediction.py     # Main script with ML pipeline
├── requirements.txt                # Dependencies
├── heart_disease_prediction.log    # Log file
│
├── models/                         # Saved models and scalers
│   ├── heart_disease_rf_model.pkl  # Trained Random Forest model
│   └── heart_disease_scaler.pkl    # Fitted StandardScaler
│
└── output/                         # Output files and visualizations
    ├── confusion_matrix.png        # Confusion matrix visualization
    ├── roc_curve.png               # ROC curve
    ├── precision_recall_curve.png  # Precision-Recall curve
    ├── model_feature_importance.png # Feature importance from model
    ├── evaluation_results.csv      # Metrics summary
    │
    └── visualizations/             # EDA visualizations
        ├── correlation_matrix.png
        ├── target_distribution.png
        ├── age_distribution.png
        ├── feature_importance.png
        └── ...
```

## 🚀 Features

- **Complete ML Pipeline**: From data loading to model evaluation
- **Exploratory Data Analysis**: Comprehensive data exploration with visualizations
- **Preprocessing**: Feature scaling and train-test splitting
- **Model Training**: Random Forest with hyperparameter tuning via GridSearchCV
- **Evaluation**: Multiple metrics (accuracy, precision, recall, F1) and visualizations
- **Logging**: Detailed logging throughout the pipeline
- **Production-Ready**: OOP design with modular components
- **Error Handling**: Robust error handling and reporting

## 📊 Results

The Random Forest model achieves strong performance in predicting heart disease:

- **Accuracy**: ~86%
- **Precision**: ~85%
- **Recall**: ~87%
- **F1 Score**: ~86%
- **ROC AUC**: ~0.92

Key findings from the analysis:
- Chest pain type (cp), maximum heart rate (thalach), and number of major vessels (ca) are the most important predictors
- There's a strong negative correlation between thalach (maximum heart rate) and heart disease
- Men are more likely to have heart disease in this dataset

## 🛠️ Installation

1. Clone this repository:
```
git clone https://github.com/yourusername/heart-disease-prediction.git
cd heart-disease-prediction
```

2. Install required dependencies:
```
pip install -r requirements.txt
```

3. Run the pipeline:
```
python heart_disease_prediction.py
```

## 📦 Requirements

- Python 3.8+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- joblib

See `requirements.txt` for specific versions.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/yourusername/heart-disease-prediction/issues).

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Contact

Your Name - [your.email@example.com](mailto:your.email@example.com)

Project Link: [https://github.com/yourusername/heart-disease-prediction](https://github.com/yourusername/heart-disease-prediction)
