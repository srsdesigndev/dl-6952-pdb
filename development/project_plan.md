# Health by the Numbers: Predicting Diabetes and BMI with Deep Learning

> **Course Project Plan** | Dataset: CDC Diabetes Health Indicators | [UCI ML Repository](https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators)

---

## Project Status

| Item | Status |
|------|--------|
| Proposal | ✅ Submitted |
| Environment Setup | ⬜ Not Started |
| Data Exploration | ⬜ Not Started |
| Baseline Models | ⬜ Not Started |
| Neural Network Models | ⬜ Not Started |
| Hyperparameter Tuning | ⬜ Not Started |
| Final Evaluation | ⬜ Not Started |
| Report / Poster | ⬜ Not Started |

---

## Research Questions

**RQ1 (Classification)**
Can we predict whether a patient has diabetes based on lifestyle and health indicators like BMI, blood pressure, cholesterol, and physical activity level?

**RQ2 (Regression)**
Can we predict a patients BMI based on lifestyle factors like age, income, physical activity, general health rating, and smoking habits?

---

## Table 1: Full Project Plan by Phase

| Phase | Exploration Area | Key Tasks | Est. Hours | Tools / Notes | Progress |
|-------|-----------------|-----------|------------|---------------|----------|
| 1 | Environment Setup | Install Python, Jupyter, PyTorch or Keras, pandas, sklearn, matplotlib. Make sure everything runs without errors. | 1 hr | Google Colab works if no local setup | ⬜ |
| 2 | Data Loading & Exploration | Download dataset from UCI. Load CSV. Check shape, column names, data types, class balance, and basic statistics. | 1.5 hrs | pandas, df.describe(), value_counts() | ⬜ |
| 3 | Data Visualization | Plot distributions of BMI, age, health rating. Check class imbalance for diabetes target. Correlation heatmap. | 1.5 hrs | matplotlib, seaborn | ⬜ |
| 4 | Data Preprocessing | Encode categorical columns, normalize numerical features, split into train/validation/test sets. | 1.5 hrs | sklearn LabelEncoder, train_test_split, StandardScaler | ⬜ |
| 5 | Baseline Models | Train Logistic Regression for classification and Linear Regression for regression. Record scores. | 2 hrs | sklearn LogisticRegression, LinearRegression | ⬜ |
| 6 | Neural Network Model 1 | Build a simple 1-hidden-layer feedforward network for both RQs. Train, validate, and record results. | 2.5 hrs | PyTorch or Keras, ReLU, Adam optimizer | ⬜ |
| 7 | Neural Network Model 2 | Build a deeper network with 2+ hidden layers, dropout, and batch normalization. Train and compare with Model 1. | 3 hrs | Dropout, BatchNorm, early stopping | ⬜ |
| 8 | Hyperparameter Tuning | Experiment with learning rate, batch size, dropout rate, and number of layers. Track which combo performs best. | 2 hrs | Manual tuning or simple grid search | ⬜ |
| 9 | Model Evaluation | Calculate recall and F1 for classification. Calculate RMSE and MAE for regression. Compare all models side by side. | 1.5 hrs | sklearn metrics, confusion matrix | ⬜ |
| 10 | Results & Writeup | Summarize findings, make charts of model performance, write final report or poster. | 3 hrs | matplotlib for plots, Word or LaTeX for report | ⬜ |

**Total Estimated Time: 13 to 18 hours**

---

## Table 2: Hyperparameter Exploration Guide

| Hyperparameter | What It Controls | Values to Try | Why It Matters |
|----------------|-----------------|---------------|----------------|
| Learning Rate | How fast the model updates its weights each step | 0.001, 0.01, 0.0001 | Too high = unstable training. Too low = very slow or stuck. |
| Batch Size | How many samples per gradient update | 32, 64, 128 | Affects training speed and how smooth the loss curve is. |
| Dropout Rate | How many neurons are randomly turned off during training | 0.2, 0.3, 0.5 | Prevents the model from memorizing the training data. |
| Hidden Layers / Neurons | Depth and width of the network | 1 layer (64), 2 layers (128, 64), 3 layers (256, 128, 64) | More layers = more capacity but also more risk of overfitting. |
| Epochs | How many full passes through the training data | 20, 50, 100 with early stopping | Too few = underfitting. Too many = overfitting. |

---

## Table 3: Model Comparison Overview

| Model | Type | Research Question | Primary Metric | Expected Difficulty |
|-------|------|------------------|----------------|---------------------|
| Logistic Regression | Baseline | Classification (RQ1) | Recall | Easy |
| Linear Regression | Baseline | Regression (RQ2) | RMSE | Easy |
| Feedforward NN (1 layer) | Neural Network | Both RQ1 and RQ2 | Recall / RMSE | Medium |
| Deep NN (2+ layers + Dropout) | Neural Network | Both RQ1 and RQ2 | Recall / RMSE | Medium |

---

## Progress Log

Use this section to log updates as you work through the project.

| Date | Phase | What Was Done | Notes |
|------|-------|---------------|-------|
| | | | |

---

## Results (fill in as you go)

### Classification (RQ1) - Diabetes Prediction

| Model | Recall | Precision | F1 Score | Accuracy |
|-------|--------|-----------|----------|----------|
| Logistic Regression (Baseline) | - | - | - | - |
| Feedforward NN (1 layer) | - | - | - | - |
| Deep NN (2+ layers) | - | - | - | - |

### Regression (RQ2) - BMI Prediction

| Model | RMSE | MAE | R2 Score |
|-------|------|-----|----------|
| Linear Regression (Baseline) | - | - | - |
| Feedforward NN (1 layer) | - | - | - |
| Deep NN (2+ layers) | - | - | - |

---

*Last updated: March 2026*