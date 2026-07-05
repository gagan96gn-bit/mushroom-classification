# Mushroom Classification

Binary classification model comparing 7 algorithms to predict whether a mushroom is edible or poisonous, based on physical characteristics.

## Overview
Uses the UCI Mushroom dataset (8,124 samples, 22 categorical features) to benchmark multiple classifiers on a real-world safety-critical classification task.

## Results
| Model | Accuracy | F1-score |
|---|---|---|
| Random Forest | 100% | 1.00 |
| Decision Tree | 100% | 1.00 |
| XGBoost | 100% | 1.00 |
| K-Nearest Neighbors | 99.6% | 0.996 |
| SVC | 97.3% | 0.973 |
| Logistic Regression | 94.8% | 0.948 |
| Gaussian Naive Bayes | 92.2% | 0.922 |

Top 3 by combined precision/recall/F1 score: Random Forest, Decision Tree, XGBoost (all scoring 1.0).

## Approach
- Label encoding for all categorical features
- Train/test split, 7 classifiers trained and evaluated in parallel
- Compared using precision, recall, F1-score, and a combined ranking metric

## Tools
Python, scikit-learn, XGBoost, pandas, seaborn

## How to run
1. Open the notebook (Colab or local Jupyter)
2. Load `mushrooms.csv` (UCI Mushroom dataset)
3. Run cells sequentially — preprocessing, model training, evaluation, comparison table
