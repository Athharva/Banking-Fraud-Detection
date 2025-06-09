# Overview
The core objective of this project is to enhance banking fraud detection performance through:
Hybrid modeling: Integration of ML classifiers (XGBoost, LightGBM, Random Forest, Logistic Regression)
Generative data augmentation using Variational Autoencoder (VAE) instead of traditional SMOTE/ADASYN
Feature engineering via VAE-based reconstruction error and fraud flagging
Hyperparameter tuning with Optuna for performance optimization
Explainable AI (XAI) to interpret model decisions


# Key Components
Baseline Models: Trained on original dataset using cross-validation
Optuna Tuning: Model-specific hyperparameter search
Data Augmentation: VAE-generated samples for minority class balancing


# Feature Engineering:
Reconstruction_Error
Flagged_as_Fraud (based on 95th percentile threshold)
Model Evaluation: ROC & PR curves, precision, recall, F1-score


# XAI Interpretability:
SHAP-based feature attribution and local explanations


# Results
Feature engineering using VAE improved recall and precision significantly, especially in minority class detection. ROC and PR curves show consistent uplift across all classifiers.


# Technologies Used
Python, Scikit-learn, XGBoost, LightGBM
Optuna for hyperparameter tuning
SHAP for XAI
Matplotlib & Seaborn for visualizations


# Paper Status
The paper titled "A Unified Hybrid ML-DL-XAI Framework for Fraud Detection using VAE-Based Augmentation and Feature Engineering" is under submission to a Scopus-indexed journal.
