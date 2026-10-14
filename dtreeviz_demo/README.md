# Decision Tree Visualization with dtreeviz

This project demonstrates how to train decision tree models and visualize their structure and predictions with `dtreeviz`. The examples use scikit-learn datasets and include both classification and regression visualizations.

## Technologies Used

- Python
- scikit-learn
- dtreeviz
- Graphviz
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

## Project Structure

- `dtreeviz_demo.ipynb` - Jupyter Notebook with the decision tree training and visualization examples.
- `cars.csv` - Input data required by the univariate and 3-D car regression examples. This file is not included in the current project folder.

## Examples

The notebook demonstrates how to:

- Train and visualize a decision tree classifier with the Iris dataset.
- Train and visualize a decision tree regressor with the Boston housing dataset.
- Change the visualization orientation and display options.
- Highlight a sample's prediction path and explain that path in plain English.
- Visualize univariate and 3-D regression trees using car data.

## Setup

Install the Python dependencies:

```bash
pip install dtreeviz scikit-learn graphviz numpy pandas matplotlib jupyter
```

The `dtreeviz` package uses Graphviz to render trees. Install the Graphviz application for your operating system as well as the Python package, and make sure the Graphviz `dot` executable is available on your PATH.

Start Jupyter Notebook from this folder and open `dtreeviz_demo.ipynb`:

```bash
jupyter notebook
```

Run the notebook cells in order. The car regression examples also require a `cars.csv` file with `WGT`, `ENG`, and `MPG` columns.

## Compatibility Notes

The notebook uses `sklearn.datasets.load_boston`, which was removed from scikit-learn 1.2, and uses the `criterion="mae"` spelling in regression examples, which newer scikit-learn versions replaced with `criterion="absolute_error"`. Those cells may need updating or a compatible scikit-learn version to run.
