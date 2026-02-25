# Human Activity Recognition using Smartphone Sensor Data

This project implements multi-class activity recognition using accelerometer and gyroscope sensor features from the UCI Human Activity Recognition dataset.

## Objective

To classify human activities (Walking, Sitting, Standing, Laying, etc.) using engineered sensor features and evaluate model performance using robust cross-validation.

---

## Dataset

- UCI Human Activity Recognition Dataset
- 561 engineered features extracted from accelerometer and gyroscope signals
- 6 activity classes

Dataset source:
https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones

---

## Methodology

1. Loaded preprocessed feature dataset (561 features)
2. Trained:
   - Logistic Regression
   - Random Forest
3. Evaluated using:
   - Accuracy
   - Classification Report
   - Confusion Matrix
   - 5-fold Cross-Validation
4. Analyzed feature importance
5. Applied PCA to study dimensionality

---

## Results

### Logistic Regression
- Test Accuracy ≈ 96%
- Cross-Validation Mean F1 ≈ 0.94
- Std Dev ≈ 0.02

### Observations
- Sitting and Standing show highest confusion
- Gravity-based acceleration features are most informative
- Gyroscope jerk features help distinguish dynamic activities

---

## Key Insights

- Static postures depend heavily on gravity orientation features.
- Dynamic activities rely on gyroscope jerk and correlation signals.
- Engineered statistical features are largely linearly separable.

---

## Tech Stack

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

---

## Author

Farha Shaikh  
BS Data Science and Applications  
Indian Institute of Technology Madras
