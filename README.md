# Bias Detection and Mitigation Framework in Machine Learning

This repository demonstrates a framework for detecting and mitigating bias in machine learning models. The focus is on analyzing and addressing gender bias in loan approval predictions using logistic regression. The project leverages fairness techniques to ensure equitable outcomes for privileged and unprivileged groups.

---

## Overview

Machine learning models can amplify biases present in training data, resulting in unfair outcomes. This project explores bias detection and mitigation techniques using a dataset containing loan application data.

Key components include:
1. **Bias Detection**: Analyze fairness and performance metrics to identify bias.
2. **Bias Mitigation**: Apply preprocessing techniques like Reweighting and Disparate Impact Remover (DIR) to mitigate bias.
3. **Post-Mitigation Evaluation**: Recalculate fairness metrics to ensure bias reduction.

---

## Features

- **Fairness Metrics**:
  - Disparate Impact (DI)
  - Statistical Parity Difference (SPD)
  - False Positive and Negative Rates (FPR/FNR) by group
- **Machine Learning**:
  - Logistic Regression for loan approval predictions
  - Evaluation using classification metrics (Precision, Recall, F1-Score)
- **Bias Mitigation Techniques**:
  - Preprocessing methods using IBM AIF360:
    - Reweighting
    - Disparate Impact Remover (DIR)
- **Impact Analysis**:
  - Evaluate the effect of swapping sensitive attributes (e.g., Gender).

---

## Results

| **Stage**              | **Disparate Impact** | **Statistical Parity Difference** |
|-------------------------|----------------------|-----------------------------------|
| **Before Training**     | 0.83                | -0.12                            |
| **After Training**      | 0.66                | -0.25                            |
| **After Mitigation**    | 0.92                | -0.06                            |

Bias mitigation significantly improves fairness by reducing adverse impacts on unprivileged groups.

---

## Technologies Used

- **Python**: Core programming language
- **Libraries**:
  - `sklearn`: Logistic regression and metrics
  - `pandas` & `numpy`: Data manipulation
  - **IBM AIF360**: Bias detection and mitigation tools
  - `matplotlib`: Data visualization

---
