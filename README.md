# Diabetes Forecasting

Predicting diabetes diagnosis from routine clinical blood and
body measurements, using 5,131 patient records and three
machine learning models.

## Problem
Early identification of high risk patients supports preventive
care. This project builds and compares classification models
that flag diabetes risk from standard blood work.

## Data
5,131 patients, 9 clinical features, binary diagnosis.
38.8 percent of patients are positive, so any useful model
must beat the 61.2 percent baseline of always guessing negative.

## Models compared
Logistic Regression: 81.2 percent accuracy, tuned with a C grid
search over 10 fold cross validation. Best performer.

K Nearest Neighbors: 79.5 percent, k selected via 10 fold cross
validation.

Decision Tree: 71.7 percent, tuned with cost complexity pruning.

## Key point
Because this predicts a serious disease, accuracy alone is not
enough. A false negative is more dangerous than a false positive,
so the model is also evaluated with a confusion matrix and recall.

## How to run
1. Clone the repo
2. pip install -r requirements.txt
3. Open notebooks/DiabetesProject.ipynb in Jupyter

## Tools
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
