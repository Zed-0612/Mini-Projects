# Mini Project 1 Personality Classification

This repository contains a Jupyter Notebook for a data science project that explores social-media behavior features and classifies users as introverted (`0`) or extroverted (`1`).

## Project workflow

The notebook covers:

1. **Data understanding** — identifies the target variable and the numerical and categorical features.
2. **Preprocessing** — checks missing values and outliers, applies one-hot encoding, and standardizes numerical features.
3. **Dimensionality reduction** — uses Principal Component Analysis (PCA) and t-distributed Stochastic Neighbor Embedding (t-SNE) for analysis and visualization.
4. **Classifier selection** — compares Logistic Regression, k-Nearest Neighbors, Decision Tree, and Random Forest.
5. **Training and tuning** — uses an 80/20 train-test split and `GridSearchCV` for hyperparameter tuning.
6. **Evaluation** — reports classification metrics and displays confusion-matrix visualizations.
7. **Interpretation and reflection** — discusses findings, limitations, and possible improvements.


## Python libraries

The notebook imports the following main libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
