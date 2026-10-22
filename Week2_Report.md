# Week 2 Project Report: Supervised Machine Learning

**Internship:** YUVAIntern – AI Pioneers Machine Learning Internship  
**Topic:** Regression and Classification using Scikit-learn

## 1. Objective

Implement supervised machine learning models, train them on labelled datasets, make predictions on held-out test data, and compare performance with suitable evaluation metrics.

## 2. Datasets and Preparation

### Titanic — Classification
The Seaborn Titanic dataset was used to predict passenger survival. The selected features were passenger class (`pclass`), age, sex, and fare; the target was `survived` (0 = did not survive, 1 = survived). Rows with missing values in the selected columns were dropped, and sex was encoded as 0 for male and 1 for female. This left 714 rows. The data was split 80/20 using `random_state=42`.

### Diabetes — Regression
Scikit-learn's built-in Diabetes dataset was used to predict a continuous target from ten input features. An 80/20 train-test split was used with `random_state=42`.

## 3. Models Implemented

**Classification:** Logistic Regression, Decision Tree Classifier, Random Forest Classifier (100 estimators), and K-Nearest Neighbors (KNN, 5 neighbors).

**Regression:** Linear Regression on the Diabetes dataset.

## 4. Evaluation Metrics

Classification models were evaluated using accuracy and classification reports containing precision, recall, and F1-score. The regression model was evaluated using Mean Squared Error (MSE) and R². Classification and regression metrics are reported separately because they assess different prediction tasks.

## 5. Classification Results

| Model | Test accuracy |
|---|---:|
| Logistic Regression | 75.52% |
| Random Forest | 74.83% |
| Decision Tree | 70.63% |
| KNN | 65.73% |

Logistic Regression produced the highest accuracy on this train-test split, with Random Forest close behind. These results apply to the selected features and split and may differ with other data or settings.

## 6. Regression Results

| Metric | Test result |
|---|---:|
| Mean Squared Error (MSE) | 2900.19 |
| R² score | 0.4526 |

The R² score indicates that the baseline model explains approximately 45.3% of the variation in the test targets. The MSE measures average squared prediction error in squared target units.

## 7. Conclusion

The work practices the core supervised-learning workflow: feature and target selection, handling missing values, train-test splitting, model fitting, prediction, evaluation, and comparison. Logistic Regression was the strongest classifier by accuracy in this experiment, and Linear Regression provided a baseline for the regression task.

## 8. Tools Used

Python, Jupyter Notebook, Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn.
