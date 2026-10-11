# Decision Tree

This project demonstrates **decision tree classification and regression** using Python and Scikit-learn. The examples are provided as Jupyter notebooks.

## Examples

### Decision Tree Classification Demo

The classification notebook contains two examples:

* Trains a `DecisionTreeClassifier` on Scikit-learn's Iris dataset
* Splits the Iris data into training and test sets (80% / 20%), predicts the test labels, and calculates accuracy
* Visualizes the trained tree
* Loads `Social_Network_Ads.csv`, encodes the `Gender` column, and uses Gender, Age, and Estimated Salary to predict whether a user purchased
* Fits a classifier with `max_depth=3` to the Social Network Ads data and visualizes the tree

The CSV contains **400 records** and the columns `User ID`, `Gender`, `Age`, `EstimatedSalary`, and `Purchased`.

### Regression Tree Example

The regression notebook:

* Loads the Boston housing dataset and uses its 13 features to predict median home value (`MEDV`)
* Splits the data into training and test sets (80% / 20%) with `random_state=42`
* Fits a `DecisionTreeRegressor` with a maximum depth of 5 and evaluates it with the R² score
* Uses `GridSearchCV` to search tree parameters, including depth, criterion, maximum features, and minimum samples per split
* Displays feature importances from the initial regression tree

> **Compatibility note:** This example uses Scikit-learn's `load_boston()` dataset loader and legacy criterion names (`mse` and `mae`). These are not supported by current Scikit-learn releases. Running this notebook may require an older Scikit-learn version, or updating the notebook to use a supported dataset and criterion names.

## Data

`Social_Network_Ads.csv` is the local dataset used by the classification notebook. The Iris dataset is loaded from Scikit-learn. The regression notebook attempts to load Boston housing from Scikit-learn.

## Libraries Used

* Python
* NumPy
* pandas
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Running the Notebooks

Install the main dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn notebook
```

Launch Jupyter Notebook from this folder and open either notebook:

```bash
jupyter notebook
```

Run the classification notebook with `Social_Network_Ads.csv` in the same folder. For the Boston regression notebook, see the compatibility note above.

## Main Concepts

* Decision Tree Classification
* Decision Tree Regression
* Training and Test Sets
* Accuracy and R² Evaluation
* Tree Visualization
* Hyperparameter Tuning
* Feature Importance
