
# Smart Health: Summer Research in Diabetes Prediction Using ML

## Duration
**Summer 2025 (1 Month)**

## Project Objective
This project demonstrates how supervised machine learning algorithms can be applied to detect early-stage **Type 2 Diabetes (T2D)** using the **UCI diabetes dataset**. It is part of a summer research initiative focused on the intersection of healthcare and AI.

---

## Project Structure

```
SmartHealth_SummerML_T2D/
├── data/                # UCI dataset and any processed versions
├── notebooks/           # Jupyter/R notebooks for EDA and modeling
├── scripts/             # Python or R scripts for model training and evaluation
├── results/             # Output metrics, plots, and reports
├── reports/             # Project summary report and slides
└── README.md            # Project documentation
```

---

## Dataset

- **Source:** UCI Machine Learning Repository  
- **Name:** [Early-stage diabetes risk prediction dataset](https://archive.ics.uci.edu/ml/datasets/Early+stage+diabetes+risk+prediction+dataset)

---

## ML Algorithms Used

The following supervised learning models will be implemented and evaluated:
- Logistic Regression (LR)
- K-Nearest Neighbors (KNN)
- Decision Tree (DT)
- Random Forest (RF)
- Support Vector Machine (SVM)
- Naïve Bayes (NB)

---

## Evaluation Metrics

We will evaluate models based on:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

---

## Key Tasks

1. Data Loading & Cleaning  
2. Exploratory Data Analysis (EDA)  
3. Feature Selection & Normalization  
4. Model Training & Evaluation  
5. Result Comparison & Conclusion

---

## Environment

- **Language:** Python 3.x or R
- **Tools:** Jupyter Notebook, RStudio  
- **Libraries:** `scikit-learn`, `pandas`, `matplotlib`, `seaborn`, `ggplot2`, etc.

---

## Outcomes

- Comparative analysis of baseline ML models on diabetes prediction.
- Insights into how lifestyle/symptom features influence prediction accuracy.
- Final report and visualizations for academic presentation or GitHub showcase.

---

- [Download Model Comparison Summary (PDF)](documents/T2D_Model_Comparison_Summary.pdf)

---

### Evaluation Summary

| Model               | Accuracy  | Precision | Recall    | F1 Score  |
|--------------------|-----------|-----------|-----------|-----------|
| Logistic Regression| 0.942308  | 0.983333  | 0.921875  | 0.951613  |
| Decision Tree      | 0.990385  | 1.000000  | 0.984375  | 0.992126  |
| Random Forest      | 0.990385  | 1.000000  | 0.984375  | 0.992126  |
| KNN                | 0.932692  | 0.983051  | 0.906250  | 0.943089  |
| SVM                | 0.990385  | 0.984615  | 1.000000  | 0.992248  |
| Naive Bayes        | 0.942308  | 0.967742  | 0.937500  | 0.952381  |

### Confusion Matrices

<img src="documents/plots/confusion_matrices.png" width="800"/>

### F1 Score Comparison

<img src="documents/plots/f1_score_comparison.png" width="600"/>

### Conclusion

- All six models performed very well, with F1 Scores above 0.94.
- SVM slightly outperformed others, achieving perfect recall and the highest F1 Score.
- Decision Tree and Random Forest also performed exceptionally with perfect precision.
- Naive Bayes performed reasonably well but slightly under the top models.
