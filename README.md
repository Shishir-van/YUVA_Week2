# YUVA Internship — Week 2: Supervised Machine Learning

## Overview
This project demonstrates supervised learning using Scikit-learn, covering classification and regression.

## Objectives
- Train classification models and compare their performance.
- Train a regression model and evaluate its predictions with regression metrics.
- Practice train/test splitting, model fitting, prediction, and evaluation.

## Models Implemented

### Classification
The Titanic dataset from Seaborn is used to predict passenger survival with these models:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbors (KNN)

The notebook compares classification accuracy and displays a bar chart. Classification reports are also printed for each model.

### Regression
The Diabetes dataset bundled with Scikit-learn is used with Linear Regression. Performance is evaluated using:
- Mean Squared Error (MSE)
- R² score

An actual-versus-predicted plot is included.

## Files
- `week2_supervised.ipynb` — notebook containing the code, evaluations, tables, and plots.
- `requirements.txt` — Python packages required to run the notebook.
- `Week2_Report.docx` — written summary of the work (add this file to the repository).

## Setup
Use Python 3.10 or newer if available.

```bash
python -m venv .venv
```

Activate the virtual environment:

**Windows**
```bash
.venv\\Scripts\\activate
```

**macOS/Linux**
```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter:

```bash
jupyter notebook
```

Open `week2_supervised.ipynb` and run the cells from top to bottom.

## Notes
- The notebook drops rows with missing values from the selected Titanic columns.
- Classification accuracy is compared separately from regression metrics because they evaluate different prediction tasks.
- Model scores can vary if the dataset, features, or train/test split are changed.
