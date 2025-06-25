# Gold Recovery Prediction Model

This project aims to predict gold recovery rates at different processing stages in a mining operation using real production data. The goal is to create a machine learning model with optimized performance based on the **sMAPE** evaluation metric, while also ensuring proper data integrity and preprocessing.

The project was completed as part of a machine learning training course.

---

## Datasets

- `gold_recovery_train.csv` — training data
- `gold_recovery_test.csv` — test data (features only)
- `gold_recovery_full.csv` — combined reference dataset (for validation)

### Features:
- Metal concentrations (Au, Ag, Pb) at various stages
- Feed and product flow measurements
- Particle sizes and recovery percentages

---

## Tools & Libraries

- Python
- pandas, numpy
- scikit-learn
- xgboost
- matplotlib, seaborn

---

## Project Steps

### 1. Data Preparation
- Checked recovery calculation and validated with MAE
- Identified and handled missing and anomalous values
- Explored feature differences between train and test sets

### 2. Data Analysis
- Studied changes in metal concentrations across purification stages
- Compared feed particle size distributions between train/test
- Evaluated and removed outliers in total concentrations

### 3. Modeling
- Wrote custom function to calculate sMAPE for evaluation
- Trained multiple regression models
- Used cross-validation to tune and evaluate models
- Selected best model based on sMAPE and tested on holdout set

---

## Business Context

- The model helps improve efficiency and planning in gold recovery pipelines.
- Target metrics are calculated using a custom symmetric mean absolute percentage error (sMAPE) function.
- Final evaluation includes predictions on both **rougher recovery** and **final output recovery**.

---

## Final Results

- Model delivered strong performance under sMAPE evaluation
- Provided reliable predictions across both key targets
- Data integrity checks ensured consistency between training and test pipelines

---

## How to Run

1. Clone this repo
2. Ensure all three CSV files are in the same directory as the notebook
3. Open the notebook in Jupyter
4. Run all cells to reproduce data prep, analysis, and model training

---

## Links

- [My LinkedIn](https://www.linkedin.com/in/ozturkkenes)
- [My GitHub](https://github.com/Harewavy)
