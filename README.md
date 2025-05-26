# Risk Models Using Tree-based Models

This project is the second assignment from the **AI for Medical Prognosis** course on Coursera (AI for Medicine Specialization by deeplearning.ai). The goal is to develop and evaluate tree-based models to predict the 10-year mortality risk using the NHANES I epidemiology dataset.

## 📊 Objective

Predict 10-year mortality risk of patients using:
- Decision Trees
- Random Forests
- Data Imputation techniques
- Model Interpretability with SHAP

## 🔍 Key Concepts Explored

- Handling Missing Data
  - Complete Case Analysis
  - Mean Imputation
  - Multivariate Imputation (IterativeImputer)
- Risk Modeling
  - Decision Trees with Hyperparameter Tuning
  - Random Forests with Grid Search
- Model Evaluation
  - C-Index for binary outcome discrimination
- Error Analysis
  - Subgroup performance breakdown
- Model Explainability
  - SHAP values and dependence plots

## 📈 Performance Metrics

| Model                          | Train C-Index | Val C-Index | Test C-Index |
|-------------------------------|---------------|-------------|--------------|
| Decision Tree (regularized)   | 0.689         | 0.630       | -            |
| Random Forest (default)       | 1.000         | 0.666       | 0.692        |
| Random Forest (mean imputed)  | 0.840         | 0.752       | 0.780        |
| Random Forest (iterative imp) | 0.877         | 0.751       | 0.783        |

## 🔬 Tools & Libraries

- Python
- pandas, numpy, seaborn, matplotlib
- scikit-learn (DecisionTreeClassifier, RandomForestClassifier, Imputers)
- SHAP (for interpretability)
- CDC NHANES I dataset
