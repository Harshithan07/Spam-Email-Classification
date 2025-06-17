# Spam Email Classification – Binary Classification with Cost-Sensitive Evaluation

## ABOUT THE PROJECT:
This project involved building and evaluating binary classifiers to detect spam emails using the UCI Spambase dataset. The objective was to compare standard accuracy-focused classification with a cost-sensitive variant, where misclassifying spam as non-spam incurs 10x the cost of the reverse. The project showcases how model performance and choice change under different real-world cost scenarios.


## USE CASE EXPLANATION:
Spam filtering is a critical task in email security and productivity. This project simulates how organizations can optimize models based not just on accuracy, but on business impact of errors. The work lies in the cybersecurity, email filtering, and cost-aware machine learning domains, supporting applications where false negatives (missed spam) are more harmful than false positives.


## HOW IT IS BUILT AND FULL WORKING:

1. Dataset: UCI Spambase dataset with 57 continuous input variables and a binary target (1 = spam, 0 = not spam).

2. Preprocessing:

- Normalized features and handled outliers.

- Split data into training and testing sets (75/25).

3. Modeling Approaches:

i. Model 1: Focused on accuracy.

- Trained Logistic Regression and Decision Tree.

- Evaluated using Accuracy, Precision, Recall, and F1-score.

ii. Model 2: Cost-sensitive.

- Applied custom cost matrix penalizing false negatives 10x more than false positives.

- Trained with Decision Tree using class_weight and adjusted thresholds.

4. Evaluation Techniques:

- Used confusion matrices and cost tables to quantify business loss.

- Compared ROC curves and Lift charts.

- Visualized model behavior with probability cutoffs.


## OUTPUT AND RESULTS OR BENCHMARKS:

- Accuracy-focused model (Model 1) achieved ~93.7% accuracy, with balanced performance but some costly false negatives.

- Cost-sensitive model (Model 2) reduced false negatives by ~50%, leading to a lower total misclassification cost despite slightly lower accuracy (~91.2%).

- Decision Tree with class weights and threshold tuning was selected as the final model.

- Demonstrated how cost-sensitive tuning improves real-world outcomes without increasing computational complexity.


## SKILLS, TOOLS:
Python, scikit-learn, Pandas, NumPy, Decision Trees, Logistic Regression, Cost-sensitive modeling, Confusion Matrix, ROC Curve, Threshold Adjustment, Classification Metrics


## KEYWORDS:
Spam filtering, binary classification, cost-sensitive learning, false negative penalty, decision tree, logistic regression, ROC curve, Lift chart, cybersecurity analytics, spam detection, scikit-learn
