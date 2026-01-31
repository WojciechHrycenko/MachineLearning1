# Machine Learning I - Portfolio Projects

![Project Status](https://img.shields.io/badge/Status-Completed-green)
![Course](https://img.shields.io/badge/Course-Machine%20Learning%201-blue)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?logo=jupyter&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit_Learn-F7931E?logo=scikit-learn&logoColor=white)
![CatBoost](https://img.shields.io/badge/Library-CatBoost-FFCC00?logo=python&logoColor=black)

## Repository Overview

This repository contains coursework and practical projects developed for the **Machine Learning 1** course. It focuses on the practical application of fundamental machine learning algorithms for both regression and classification tasks.

The repository is divided into two main projects, each containing:
* **Full Analysis:** Complete workflow including EDA, feature engineering, and model tuning.
* **Short Version (Inference):** A streamlined notebook focused on the final model pipeline and generating predictions.
* **Presentation:** A slide deck summarizing the business problem and results.

## Authors & Roles

* **Wojciech Hrycenko** – **Classification Project** (Insurance Claims)
* **Cezary Kuźmowicz** – **Regression Project** (Apartment Prices)

---

## Project 1: Apartment Price Prediction
**Folder:** `Apartments/`
**Lead:** Cezary Kuźmowicz

### Objective
The goal was to predict apartment prices based on location, size, and amenities. The analysis focused on handling outliers, feature engineering, and applying regularization techniques to prevent overfitting.

### Key Files
* **`Regression_1_Full_Analysis.ipynb`**:
    * Detailed Exploratory Data Analysis (EDA).
    * Comparison of Linear Regression vs. Regularized models (Lasso, Ridge, ElasticNet).
    * Feature importance analysis using coefficients.
* **`Regression_2_Short_Version.ipynb`**:
    * Final model implementation (Inference).
    * Generation of predictions for the test dataset (`final_predictions_regression.csv`).
* **`Presentation/Apartments Regression Presentation.pptx`**: Summary slides.

### Key Techniques
* **Regularization (L1/L2):** Used to handle multicollinearity and prevent overfitting.
* **Log-transformation:** Applied to the target variable to correct skewness.

---

## Project 2: Insurance Claim Classification
**Folder:** `Insurances/`
**Lead:** Wojciech Hrycenko

### Objective
This project tackles a binary classification problem: predicting whether a customer will file a travel insurance claim. The focus was on handling imbalanced data and utilizing advanced tree-based gradient boosting methods.

### Key Files
* **`Insurance_For_Classification Full.ipynb`**:
    * In-depth analysis of risk factors (EDA).
    * Preprocessing pipeline design (Categorical Encoding).
    * Model training and hyperparameter tuning using **CatBoost Classifier**.
* **`Insurance_For_Classification Short.ipynb`**:
    * Loading the optimized pipeline.
    * Generating probabilities and class labels for the test set (`insurance_test_with_predictions.csv`).
* **`presentation/Insurance Classification Presentation.pptx`**: Summary slides.

### Key Techniques
* **Gradient Boosting (CatBoost):** Chosen for its superior handling of categorical features.
* **Pipeline Optimization:** Automated preprocessing and inference flow using `sklearn` pipelines.

---

## Technologies

The projects were developed in **Python**, utilizing the following stack:

* **Scikit-learn:** Data preprocessing, pipelines, linear models, and metrics.
* **CatBoost:** Gradient boosting for classification.
* **Pandas & NumPy:** Data manipulation.
* **Matplotlib & Seaborn:** Data visualization.
* **Statsmodels:** Statistical tests and analysis.

## Usage Instructions

1.  Clone the repository.
2.  Install dependencies (ensure `catboost` and `sklearn` are installed).
3.  Navigate to the respective project folder (`Apartments` or `Insurances`).
4.  Run the **Full Analysis** notebook to understand the methodology or the **Short Version** to see the model in action.
