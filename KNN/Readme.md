# K-Nearest Neighbors on Breast Cancer Dataset

This project implements **K-Nearest Neighbors (KNN) Classification** on the Breast Cancer Wisconsin dataset using Python and Scikit-learn.

## Data Used

I used the **Breast Cancer Wisconsin (Diagnostic) dataset** from Kaggle.

The dataset was loaded from:

```python
breast-cancer-wisconsin-data/data.csv
```

Before training the model, I removed the following columns:

- `id`
- `Unnamed: 32`

The remaining data was divided into:

- **Features (`X`)** — 30 medical features
- **Target (`y`)** — diagnosis (`M` / `B`)

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
- Implemented **KNN Classification**
- Initially used `k = 3`
- Calculated the model accuracy
- Tested different values of `k` from **1 to 15**
- Plotted accuracy for different `k` values
- Visualized KNN decision boundaries using the first two features
- Added an interactive visualization to observe the effect of different `k` values

## Libraries Used