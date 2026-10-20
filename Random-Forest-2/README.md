# Random Forest Demo

This project uses a Jupyter notebook to demonstrate Random Forest classification and regression with synthetic data. It compares each Random Forest with a single decision tree and visualizes the models' predictions.

## Notebook

`random_forest_demo.ipynb` contains two demonstrations:

### Classification

- Generates 500 two-dimensional samples using scikit-learn's `make_circles`
- Splits the data into training and test sets (80% training, 20% test)
- Plots the generated classes
- Fits a `DecisionTreeClassifier` and a `RandomForestClassifier`
- Visualizes each model's predicted decision regions
- Uses 500 trees in the Random Forest classifier

### Regression

- Generates noisy synthetic data from a function made from two Gaussian-shaped curves
- Uses 150 training samples and 1,000 test samples, with noise level 0.1
- Fits a `DecisionTreeRegressor` and a `RandomForestRegressor`
- Plots both predictions alongside the underlying function and training samples
- Uses 1,000 trees in the Random Forest regressor

The notebook labels the regression error as MSE, but calculates the **sum of squared errors** (SSE) rather than dividing by the number of test samples.

## Requirements

- Python 3
- Jupyter Notebook
- NumPy
- Matplotlib
- scikit-learn

Install the dependencies with:

```bash
pip install numpy matplotlib scikit-learn notebook
```

## Run

From this directory, start Jupyter Notebook:

```bash
jupyter notebook
```

Open `random_forest_demo.ipynb` and run the cells from top to bottom. All data is generated in the notebook; no external dataset is required.
