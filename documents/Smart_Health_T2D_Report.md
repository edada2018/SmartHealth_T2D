
# Smart Health T2D Report

## Objective

This project focuses on evaluating and comparing the performance of various baseline supervised machine learning models for early-stage detection of Type 2 Diabetes (T2D). Using clinical symptom-based data from the UCI dataset, we aim to assess the predictive power of six common algorithms in identifying T2D risk. The goal is to determine which models offer the best accuracy, precision, recall, and F1-score, providing insight into their suitability for potential integration into non-invasive, data-driven health screening systems.

## Dataset and Preprocessing

- Data Source: UCI Early Stage Diabetes Risk Prediction Dataset
- Total Records: 520
- Target Variable: `class` (Positive/Negative diagnosis)
- Preprocessing Steps:
  - Encoded categorical features (e.g., 'Yes'/'No', 'Male'/'Female')
  - Scaled numeric feature 'Age' using StandardScaler
  - Train-Test Split (80%-20%)

## Baseline Models Trained

- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Naive Bayes

## Evaluation Summary

| Model               | Accuracy | Precision | Recall | F1 Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 0.942308 | 0.983333  | 0.921875 | 0.951613 |
| Decision Tree       | 0.990385 | 1.000000  | 0.984375 | 0.992126 |
| Random Forest       | 0.990385 | 1.000000  | 0.984375 | 0.992126 |
| KNN                 | 0.932692 | 0.983051  | 0.906250 | 0.943089 |
| SVM                 | 0.990385 | 0.984615  | 1.000000 | 0.992248 |
| Naive Bayes         | 0.942308 | 0.967742  | 0.937500 | 0.952381 |

## Confusion Matrices

![Confusion Matrix](plots/confusion_matrices.png)

## F1 Score Comparison

![F1 Score Comparison](plots/f1_score_comparison.png)

## Conclusion

- All six models performed very well, with F1 Scores above 0.94.
- SVM slightly outperformed others, achieving perfect recall and highest F1 Score.
- Decision Tree and Random Forest also performed exceptionally with perfect precision.
- Naive Bayes performed reasonably well but slightly under the top models.

## Next Steps

- Perform hyperparameter tuning (already completed except for Naive Bayes)
- Save and load trained models using joblib
- Integrate into a health application pipeline

## File Structure

```
├── Final_SmartHealth_T2D_Modeling.ipynb  # Main notebook
├── plots/
│   ├── confusion_matrices.png
│   └── f1_score_comparison.png
├── ucidata.csv                           # Dataset
```
