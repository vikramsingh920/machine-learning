# Voting Ensemble: Classification and Regression

This project demonstrates how voting ensembles combine multiple machine-learning models for classification and regression. The notebooks compare individual estimators with ensemble predictions using cross-validation.

## Technologies Used

- Python
- NumPy
- Pandas
- Seaborn
- scikit-learn
- Jupyter Notebook

## Project Structure

- `voting-classifier-iris.ipynb` - Builds voting classifiers for the Iris dataset and compares hard, soft, and weighted voting. It also demonstrates soft voting with several SVC models.
- `voting_regressor.ipynb` - Builds voting regressors from linear regression, decision tree, and SVR models, then explores weighted voting and decision trees with different depths.
- `README.md` - Project documentation.

## Getting Started

Install the dependencies in an environment with a compatible Python version:

```bash
pip install numpy pandas seaborn "scikit-learn<1.2" jupyter
```

Start Jupyter Notebook and open either notebook:

```bash
jupyter notebook
```

### Dataset notes

- The classifier notebook expects the Iris CSV at `/kaggle/input/iris/Iris.csv`, as it was written for Kaggle. To run it elsewhere, provide the path to your copy of `Iris.csv`. The file should contain `Id`, `Species`, and the Iris measurement columns.
- The regressor notebook uses scikit-learn's `load_boston` dataset loader. That loader was removed in scikit-learn 1.2, so this notebook requires scikit-learn earlier than 1.2 unless the dataset-loading code is updated.

## Methods

### Classification

The classifier notebook uses Logistic Regression, Random Forest, and K-Nearest Neighbors as the base estimators. It evaluates each model and the voting ensembles with 10-fold cross-validation and accuracy:

- **Hard voting** selects the class predicted by the majority of estimators.
- **Soft voting** averages predicted class probabilities and selects the class with the highest combined probability.
- **Weighted voting** assigns different weights to estimators during soft voting.

The notebook also compares several polynomial-kernel SVC models and combines them with soft voting.

### Regression

The regressor notebook combines Linear Regression, Decision Tree Regression, and Support Vector Regression. It evaluates the base models and ensembles using 10-fold cross-validation and the R² score. It also experiments with estimator weights and a voting ensemble of decision trees with different maximum depths.
