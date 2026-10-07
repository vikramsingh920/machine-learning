
# K-Nearest Neighbors on Breast Cancer Dataset

This project implements **K-Nearest Neighbors (KNN) Classification** on the Breast Cancer Wisconsin dataset using Python and Scikit-learn.

## Data Used

I used the **Breast Cancer Wisconsin (Diagnostic) dataset**.

The dataset was loaded from the Kaggle input file:

```python
/kaggle/input/breast-cancer-wisconsin-data/data.csv
```

Before training the model, I removed:

- `id`
- `Unnamed: 32`

The remaining data contains:

- **30 features**
- **569 samples**
- Target: `diagnosis` (`M` / `B`)

The data was split into:

- **80% training data**
- **20% testing data**
- `random_state = 2`

The features were standardized using `StandardScaler`.

## What I Did

- Loaded the Breast Cancer dataset
- Removed unnecessary columns
- Split the data into training and testing sets
- Standardized the features
- Applied KNN Classification
- Initially used `k = 3`
- Calculated the model accuracy
- Tested different values of `k` from **1 to 15**
- Plotted accuracy for different values of `k`
- Used Scikit-learn's built-in Breast Cancer dataset for visualization
- Created an interactive decision boundary visualization for different `k` values

## Libraries Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- ipywidgets

## Main Concepts

- K-Nearest Neighbors
- Classification
- Feature Scaling
- Standardization
- Train-Test Split
- Accuracy Score
- Choosing the value of `k`
- Decision Boundaries