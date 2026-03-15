# Health by the Numbers: Predicting Diabetes and BMI with Deep Learning

A deep learning course project using the CDC Diabetes Health Indicators dataset to predict diabetes diagnosis and BMI from patient lifestyle and health data.

---

## Dataset

**CDC Diabetes Health Indicators**
Source: [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators)
- 253,680 rows, 22 features
- Tabular CSV, no missing values

---

## Research Questions

- **Classification:** Can we predict whether a patient has diabetes based on lifestyle and health indicators?
- **Regression:** Can we predict a patients BMI based on demographic and lifestyle factors?

---

## Models

| Task | Baseline | Model 1 | Model 2 |
|------|----------|---------|---------|
| Classification | Logistic Regression | Feedforward NN (1 layer) | Deep NN (2+ layers + Dropout) |
| Regression | Linear Regression | Feedforward NN (1 layer) | Deep NN (2+ layers + Dropout) |

---

## Project Plan

See [PROJECT_PLAN.md](./development/project_plan.md) for the full phase breakdown, hyperparameter guide, and progress tracking.

---

## Tech Stack

Python, PyTorch, pandas, scikit-learn, matplotlib, seaborn