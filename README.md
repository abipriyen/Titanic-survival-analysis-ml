# Titanic Survival Prediction using Machine Learning

An end-to-end Machine Learning project that predicts passenger survival on the Titanic using multiple classification algorithms, robust data preprocessing techniques, Scikit-Learn Pipelines, and Hyperparameter Tuning. The project follows a complete machine learning workflow from data preprocessing to model evaluation while identifying the best-performing classification model.

---

# Project Overview

The objective of this project is to predict whether a passenger survived the Titanic disaster based on demographic and travel-related information. Multiple machine learning algorithms were trained, evaluated, and compared using standard evaluation metrics. After comprehensive analysis, the best-performing model was selected through Hyperparameter Tuning.

The entire workflow follows industry-standard machine learning practices to create a clean, reproducible, and scalable pipeline.

---
# Model Evaluation Overview

Three supervised machine learning classification algorithms were implemented and evaluated using the same preprocessing pipeline to ensure a fair comparison.

| Model | Evaluation Status | Hyperparameter Tuning |
|--------|-------------------|-----------------------|
| Logistic Regression | ✅ Trained & Evaluated | ❌ Not Applied |
| Gaussian Naive Bayes | ✅ Trained & Evaluated | ❌ Not Applied |
| Decision Tree Classifier | ✅ Trained & Evaluated | ✅ GridSearchCV |

The performance of each model was assessed using:

- Classification Report
- Precision
- Recall
- F1-Score
- Training Accuracy
- Testing Accuracy

After comparing all models, the Decision Tree Classifier demonstrated the best overall performance. Hyperparameter Tuning using **GridSearchCV** was then applied to further optimize the model. The tuned Decision Tree achieved improved predictive performance and demonstrated good generalization on unseen data.

---

## Model Evaluation Results

### Logistic Regression

<p align="center">
  <img src="Model evaluation/LogisticRegression.png" width="850">
</p>

---

### Gaussian Naive Bayes

<p align="center">
  <img src="Model evaluation/GaussianNB.png" width="850">
</p>

---

### Decision Tree Classifier

<p align="center">
  <img src="Model evaluation/DecisionTreeClassifier.png" width="850">
</p>

# Project Objectives

- Predict passenger survival accurately.
- Build a complete machine learning workflow.
- Compare multiple classification algorithms.
- Perform proper data preprocessing.
- Improve model performance using Hyperparameter Tuning.
- Select the best-performing model.
- Analyze feature importance.

---

# Dataset

**Dataset:** Titanic Survival Dataset

**Target Variable**

| Value | Meaning |
|--------|----------|
| 0 | Did Not Survive |
| 1 | Survived |

---

# Complete Project Workflow

```
Dataset Collection
        │
        ▼
Data Loading
        │
        ▼
Initial Data Inspection
        │
        ▼
Duplicate Value Checking
        │
        ▼
Missing Value Analysis
        │
        ▼
Feature Selection
        │
        ▼
Train-Test Split
        │
        ▼
Missing Value Imputation
        │
        ▼
One-Hot Encoding
        │
        ▼
Feature Scaling
        │
        ▼
ColumnTransformer
        │
        ▼
Pipeline Construction
        │
        ▼
Multiple Machine Learning Models
        │
        ▼
Model Evaluation
(Classification Report,
Train Score,
Test Score)
        │
        ▼
Hyperparameter Tuning
        │
        ▼
Best Model Selection
        │
        ▼
Feature Importance Analysis
```

---

# Data Preprocessing Techniques

The following preprocessing techniques were applied:

- Data Loading
- Dataset Inspection
- Duplicate Value Checking
- Missing Value Analysis
- Mean Imputation using SimpleImputer
- Feature Selection
- Train-Test Split
- One-Hot Encoding for Categorical Features
- StandardScaler for Numerical Features
- ColumnTransformer
- Scikit-Learn Pipeline

---

# Main Pipeline

```
Input Data
      │
      ▼
SimpleImputer
      │
      ▼
ColumnTransformer
      │
      ├────────► OneHotEncoder
      │
      └────────► StandardScaler
      │
      ▼
Machine Learning Model
      │
      ▼
Prediction
```

---

# Machine Learning Models Used

The following classification algorithms were implemented and compared:

- Logistic Regression
- Gaussian Naive Bayes
- Decision Tree Classifier

Each model was trained using the same preprocessing pipeline to ensure fair comparison.

---

# Initial Model Evaluation

Before Hyperparameter Tuning, each machine learning model was evaluated using:

- Classification Report
- Training Accuracy
- Testing Accuracy

The comparison focused on:

- Prediction Accuracy
- Precision
- Recall
- F1-Score
- Generalization Ability

This evaluation helped identify the most promising model for optimization.

---

# Hyperparameter Tuning

Hyperparameter Tuning was performed using **GridSearchCV** to optimize the Decision Tree Classifier.

The tuning process included:

- Cross Validation
- Grid Search
- Multiple Parameter Combinations
- Best Parameter Selection

The optimized model demonstrated improved predictive performance compared to the default configuration.

---

# Final Model Selection

After comparing all machine learning algorithms and optimizing the Decision Tree Classifier through Hyperparameter Tuning, the tuned Decision Tree model was selected as the final model because it achieved the best predictive performance on the dataset.

The selected model demonstrated:

- Strong Classification Performance
- High Training Accuracy
- High Testing Accuracy
- Good Generalization on unseen data

---

# Feature Importance Analysis

Feature importance analysis was performed using the optimized Decision Tree model to identify the most influential features contributing to survival prediction.

This analysis provides better interpretability of the trained model.

---

# Model Evaluation

The final model was evaluated using:

- Classification Report
- Train Accuracy
- Test Accuracy
- Feature Importance
- Correlation Heatmap

---

# Technologies Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn

---

# Machine Learning Techniques Used

- Supervised Machine Learning
- Binary Classification
- Missing Value Imputation
- SimpleImputer
- One-Hot Encoding
- StandardScaler
- ColumnTransformer
- Scikit-Learn Pipeline
- Model Comparison
- Hyperparameter Tuning
- GridSearchCV
- Cross Validation
- Feature Importance Analysis

---

# Project Highlights

- End-to-End Machine Learning Workflow
- Data Cleaning and Missing Value Handling
- Feature Engineering
- One-Hot Encoding
- StandardScaler
- ColumnTransformer
- Scikit-Learn Pipeline
- Multiple Model Comparison
- Logistic Regression
- Gaussian Naive Bayes
- Decision Tree Classifier
- Hyperparameter Tuning using GridSearchCV
- Best Model Selection
- Feature Importance Analysis
- Correlation Heatmap Visualization

---

# Future Improvements

- Perform advanced feature engineering.
- Explore ensemble learning techniques.
- Implement Random Forest and XGBoost.
- Build a Streamlit or FastAPI web application.
- Deploy the model to the cloud.

---

# Conclusion

This project demonstrates a complete end-to-end machine learning workflow for Titanic Survival Prediction using industry-standard preprocessing and model development techniques. Multiple classification algorithms—including Logistic Regression, Gaussian Naive Bayes, and Decision Tree Classifier—were developed and evaluated using Classification Reports along with Training and Testing Scores.

After comparing the models, Hyperparameter Tuning was applied to the Decision Tree Classifier using GridSearchCV to improve its performance. The optimized model achieved the best overall predictive performance and demonstrated good generalization on unseen data.

By integrating preprocessing, Scikit-Learn Pipelines, model comparison, hyperparameter optimization, and feature importance analysis, this project provides a scalable and reproducible machine learning solution suitable for portfolio and learning purposes.
