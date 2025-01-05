# Comparative Analysis of Protein Classification Pipelines for Ewing's Sarcoma Biomarker Detection
# Project Overview
  This project involves a comparative analysis of two pipelines for classifying protein samples into "Control" and "Cancerous" groups, focusing on identifying candidate biomarkers for Ewing's Sarcoma. The study is based on data from a research paper that used statistical testing (ANOVA and T-test) to identify Differentially Expressed Proteins (DEPs) between the two groups.

The proposed pipeline introduces several improvements over the paper’s approach by incorporating:
  Advanced preprocessing methods such as imputation and normalization.
  Modern machine learning techniques like MRMR and Recursive Feature Elimination (RFE) for feature selection.
  Cross-validation and resampling with SMOTE to handle class imbalance.
  Model evaluation using SVM and Random Forest with hyperparameter optimization.
This project aims to enhance biomarker detection by comparing the effectiveness of our pipeline against the paper’s pipeline in identifying common features and improving classification performance.

# Installation Instructions
- Check this repository.
- Install the required dependencies in requirements.txt.

# Usage
-Preprocessing: The script preprocesses the protein expression data by:
  Filtering features with more than 40% missing values.
  Imputing missing values using the mean.
  Normalizing the data row-wise by the median and column-wise using Z-score normalization.
-Feature Selection:
  MRMR: Selects features based on relevance and redundancy minimization.
  RFE: Recursively eliminates features based on a machine learning model's performance.
-Model Training and Evaluation:
  Applies SVM and Random Forest with hyperparameter optimization using GridSearchCV.
  Evaluates models with metrics such as Accuracy and ROC AUC.

# Additional information 
- The data preprocessing and feature selection steps are implemented in Python. Use scikit-learn, pandas, and TensorFlow in your Python environment or Google Colab for execution.
- For more instructions, see the code and the documentation provided in this repository.
