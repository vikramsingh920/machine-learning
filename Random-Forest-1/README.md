# Random Forest Classification

This project uses a Jupyter notebook to explore classification on a heart-disease dataset. It compares several classifiers, evaluates a Random Forest with a holdout set and cross-validation, and tunes its hyperparameters with grid and randomized search.

## Notebook

`code-example-random-forest.ipynb` covers:

- Loading and inspecting the dataset
- Splitting features and the target into training and test sets
- Comparing Random Forest, Gradient Boosting, SVC, and Logistic Regression classifiers
- Evaluating accuracy on a held-out test set
- Evaluating a Random Forest with 10-fold cross-validation
- Tuning Random Forest hyperparameters with `GridSearchCV` and `RandomizedSearchCV`

## Dataset

The notebook reads a file named `heart.csv` from the current working directory. That CSV is not included in this project folder, so add the dataset file before running the notebook.

The notebook expects 14 columns: 13 input features followed by a `target` column. The target is used as the label, and all preceding columns are used as features. The saved notebook output shows 303 rows.

## Requirements

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn

Install the dependencies with:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn notebook
```

## Run

From this directory, start Jupyter:

```bash
jupyter notebook
```

Open `code-example-random-forest.ipynb`, ensure `heart.csv` is in the notebook's working directory, and run the cells from top to bottom.

## Recorded results

The notebook's saved holdout-test accuracies are:

| Model | Accuracy |
| --- | ---: |
| Random Forest (default settings) | 85.25% |
| Gradient Boosting | 77.05% |
| Support Vector Classifier | 70.49% |
| Logistic Regression | 88.52% |
| Random Forest (`max_samples=0.75`) | 90.16% |

These are the recorded results from one 80/20 train-test split (`random_state=42`); they may vary with dataset or library versions. The notebook also runs cross-validation and hyperparameter searches, which report separate scores.
