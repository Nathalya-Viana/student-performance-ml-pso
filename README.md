# Student Performance Prediction using Machine Learning and PSO

## Overview

This project investigates the prediction of students' final grades using Machine Learning techniques. The objective was to compare the performance of Support Vector Machine (SVM) and Random Forest Regressor (RFR) models optimized through Particle Swarm Optimization (PSO).

The study evaluates different preprocessing strategies and validates the results using statistical tests.

---

## Dataset

Source: UCI Machine Learning Repository

Dataset: Student Performance Dataset

The dataset contains demographic, social, and academic information from secondary school students.

### Target Variable

- G3 (Final Grade)

### Selected Features

- Age
- Study Time
- Failures
- Absences
- Parents' Education
- Family Support
- Previous Grades (G1 and G2)

---

## Project Objectives

- Predict students' final grades.
- Compare SVM and Random Forest models.
- Optimize hyperparameters using PSO.
- Evaluate model performance using regression metrics.
- Perform statistical validation through the Wilcoxon test.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- PySwarms
- SciPy
- Matplotlib
- Jupyter Notebook

---

## Methodology

### 1. Data Preparation

The dataset was analyzed and prepared for machine learning experiments.

Two scenarios were evaluated:

- Original Dataset
- Preprocessed Dataset

### 2. Hyperparameter Optimization

Particle Swarm Optimization (PSO) was applied to find optimal hyperparameters.

#### Support Vector Machine (SVM)

- C
- Gamma

#### Random Forest Regressor (RFR)

- Number of Estimators
- Maximum Depth
- Minimum Samples Split

### 3. Model Training

The following models were trained and evaluated:

- SVM (Original Data)
- SVM (Preprocessed Data)
- Random Forest (Original Data)
- Random Forest (Preprocessed Data)

### 4. Evaluation Metrics

Performance was measured using:

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)

### 5. Statistical Validation

The Wilcoxon Signed-Rank Test was used to verify whether the differences between model performances were statistically significant.

---

## Results

### R² Score Comparison

| Model | R² |
|---------|---------|
| Random Forest (Original Data) | 0.8566 |
| SVM (Original Data) | 0.8329 |
| SVM (Preprocessed Data) | 0.8273 |
| Random Forest (Preprocessed Data) | 0.8254 |

### Lowest Prediction Error

| Model | MAE |
|---------|---------|
| SVM (Preprocessed Data) | 0.8639 |

---

## Results Discussion

### Random Forest Performance

Random Forest trained on the original dataset achieved the highest R² score, demonstrating superior predictive capability.

The results suggest that preprocessing did not improve Random Forest performance, which is expected because tree-based algorithms are generally insensitive to feature scaling.

### SVM Performance

The SVM model benefited from preprocessing and achieved the lowest Mean Absolute Error.

This behavior is consistent with the characteristics of SVM, which is sensitive to feature scales.

### Statistical Analysis

The Wilcoxon test indicated statistically significant differences between the evaluated configurations, supporting the reliability of the observed results.

---

## Key Findings

- Random Forest achieved the highest predictive performance.
- SVM achieved the lowest prediction error after preprocessing.
- Preprocessing improved SVM performance.
- Random Forest performed better using the original dataset.
- Statistical tests confirmed the significance of the results.

---


