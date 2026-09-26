# Outlier Detection Using IQR

This notebook is created for **learning and understanding the IQR (Interquartile Range) method for outlier detection**.

The main purpose of this notebook is to understand how outliers can be identified using statistical techniques and how they can be handled using Pandas.

## What I Learned

* What outliers are
* How to visualize outliers using boxplots
* Understanding the 25th percentile (Q1)
* Understanding the 75th percentile (Q3)
* Calculating the Interquartile Range (IQR)
* Calculating the lower and upper limits
* Identifying outliers using the IQR method
* Removing outliers from a DataFrame

## IQR Method

The Interquartile Range is calculated as:

```text
IQR = Q3 - Q1
```

The outlier boundaries are:

```text
Lower Limit = Q1 - 1.5 × IQR
Upper Limit = Q3 + 1.5 × IQR
```

Values below the lower limit or above the upper limit are considered potential outliers.

## Notebook

The notebook uses a placement dataset and applies the IQR method to the `placement_exam_marks` column.

The notebook covers the complete process:

```text
Dataset
   ↓
Data Visualization
   ↓
Boxplot
   ↓
Calculate Q1 and Q3
   ↓
Calculate IQR
   ↓
Calculate Lower & Upper Limits
   ↓
Identify Outliers
   ↓
Remove Outliers
   ↓
Compare the Data
```

## Libraries Used

* NumPy
* Pandas
* Matplotlib
* Seaborn

## Purpose

This is a **practice/learning notebook**, created while learning the fundamentals of **data preprocessing and outlier detection in Machine Learning**.

It is not intended to be a production ML project.
