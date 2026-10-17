# Bagging Ensemble Learning

This project explores bootstrap aggregating (Bagging) and related ensemble techniques using scikit-learn. It includes interactive notebook experiments covering classification, regression, and ensemble variants such as pasting, random subspaces, and random patches.

## Project goal

The notebooks in this repository demonstrate how bagging improves model stability and reduces variance by training multiple learners on bootstrap samples and aggregating their predictions.

## What is covered

- Bagging for classification
- Bagging for regression
- Pasting
- Random subspaces
- Random patches
- Out-of-bag (OOB) evaluation
- Hyperparameter tuning with GridSearchCV

## Notebook overview

### 1. bagging_demo.ipynb

A practical introduction to BaggingClassifier using synthetic classification data.

Topics covered:
- Decision tree baseline
- Bagging with decision trees
- Bagging with SVM as the base estimator
- Sample and feature resampling behavior
- Accuracy comparisons

### 2. bagging_regression.ipynb

A regression-focused notebook using the Boston housing dataset (or equivalent dataset in newer environments).

Topics covered:
- Linear Regression, Decision Tree, and KNN baselines
- BaggingRegressor performance
- R² score evaluation
- GridSearchCV for ensemble tuning

### 3. bagging-learning-tool.ipynb

A case-study notebook focused on a classification task using the Iris dataset.

Topics covered:
- Data preprocessing and encoding
- Feature selection for a two-class problem
- Bagging-based experimentation
- Random subspaces and random patches strategies

## Key concepts

### Bagging

Bagging creates multiple models trained on bootstrap samples of the training data. Each model makes a prediction, and the final prediction is aggregated (for example by majority vote for classification or averaging for regression).

### Pasting

Pasting is similar to bagging, but it samples without replacement, which means the bootstrap draw is not used.

### Random subspaces

Random subspaces train base models on random subsets of features, which helps when data is high-dimensional.

### Random patches

Random patches sample both rows and columns, combining row-wise and feature-wise randomness.

### Out-of-bag score

Some bagging implementations can estimate generalization performance using the subset of samples that were not selected in a given bootstrap sample.

## Setup

### Requirements

- Python 3.9+
- Jupyter Notebook or VS Code with Jupyter support
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

### Install dependencies

```bash
pip install numpy pandas scikit-learn matplotlib seaborn notebook
```

## Run the project

1. Open the notebooks in Jupyter or VS Code.
2. Run the cells from top to bottom.
3. Compare the baseline model performance to the bagging results.

You can also launch Jupyter with:

```bash
jupyter notebook
```

## Notes

- Bagging usually improves performance when the base estimator is high-variance and unstable.
- For high-dimensional datasets, random subspaces and random patches are often useful.
- Hyperparameter tuning can help identify a better sampling strategy for specific datasets.
- Some older examples may use deprecated scikit-learn APIs depending on the installed version.

## Repository structure

```text
Bagging/
├── README.md
├── bagging_demo.ipynb
├── bagging_regression.ipynb
├── bagging-learning-tool.ipynb
```

## Recommended learning flow

1. Start with bagging_demo.ipynb to understand the core ideas.
2. Move to bagging_regression.ipynb for regression behavior and model comparison.
3. Explore bagging-learning-tool.ipynb for a dataset-driven practice example.

## License

This project is intended for educational and experimental use.
