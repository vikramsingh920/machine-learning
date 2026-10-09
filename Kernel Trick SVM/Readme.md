# Kernel Trick in Support Vector Machines (SVM)

This project explores the **Kernel Trick in SVM** using Python and Scikit-learn. I compared linear, RBF, and polynomial kernels on a non-linearly separable dataset.

## Data Used

I generated a synthetic dataset using Scikit-learn's `make_circles()` function.

```python
from sklearn.datasets import make_circles

X, y = make_circles(100, factor=0.1, noise=0.1)
```

### Dataset Details
- **100 samples**
- **2 input features**
- **2 classes**
- `factor = 0.1`
- `noise = 0.1`

The dataset contains circular patterns, making it useful for understanding non-linear classification.

## What I Did

- Generated and visualized the circular dataset
- Split the data into 80% training and 20% testing sets
- Implemented SVM with a linear kernel
- Applied the **RBF kernel**
- Applied a polynomial kernel with degree 2
- Evaluated the models using accuracy score
- Plotted decision boundaries for each kernel
- Visualized the data in 3D to explore feature transformation

## Libraries Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Main Concepts

- Support Vector Machines (SVM)
- Kernel Trick
- Linear Kernel
- RBF Kernel
- Polynomial Kernel
- Decision Boundaries
- Model Accuracy
