# Personality Prediction Pipeline

## Overview

This project provides a comprehensive, production-ready pipeline for predicting personality type (Extrovert vs. Introvert) from behavioral survey data. The workflow includes advanced data cleaning, imputation, class balancing, feature engineering, model training, and ensemble prediction, following best practices in data science and machine learning.

## Dataset Source

The original dataset for this project is available from the Kaggle competition:
[https://www.kaggle.com/competitions/playground-series-s5e7/data](https://www.kaggle.com/competitions/playground-series-s5e7/data)

## Workflow Summary

- **Data Exploration:** In-depth EDA, visualization, and statistical analysis to understand feature-target relationships and data quality issues.
- **Missing Value Handling:** Advanced multiple imputation (ensemble-based) to address MAR (Missing At Random) patterns, with quality validation.
- **Class Imbalance:** Robust balancing using SMOTE, ADASYN, and class weighting, with synthetic data quality checks.
- **Feature Engineering:** Creation of domain-specific interaction features and composite scores, advanced transformations, and rigorous feature selection.
- **Modeling:** Training and evaluation of multiple models (Random Forest, XGBoost, LightGBM, SVM, MLP, etc.) with PCA for dimensionality reduction. Final predictions are made using a weighted ensemble of top models.
- **Outputs:** Cleaned datasets, encoders, and prediction files are saved for reproducibility and deployment.

## File

- `personality_prediction.ipynb`: Main notebook containing the full pipeline, analysis, and results.


## Usage

1. **Requirements:**

   - Python 3.8+
   - Jupyter Notebook
   - Key packages: pandas, numpy, scikit-learn, xgboost, lightgbm, imbalanced-learn, shap, matplotlib, seaborn

2. **Running the Pipeline:**

   - Open `personality_prediction.ipynb` in Jupyter.
   - Run all cells sequentially to reproduce the full workflow, from EDA to final predictions.
   - Outputs and artifacts will be saved in the project directory.

3. **Customizing/Extending:**
   - Adjust feature engineering or model parameters in the notebook as needed.
   - Use the saved encoder (`target_encoder.pkl`) to decode model predictions.

## Results

- The final ensemble model achieves a balanced accuracy of ~95.8% (cross-validated), demonstrating strong predictive power and robust generalization.
- The pipeline is modular, well-documented, and ready for further optimization or deployment.

## Contact

For questions or collaboration, please contact the project maintainer.
