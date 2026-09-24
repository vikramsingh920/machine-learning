# Naive Bayes

This project demonstrates **Naive Bayes Classification** using Python and Pandas.

## Data Used

I used the **Play Tennis dataset** from `play_tennis.csv`.

The dataset contains **14 observations** with the following features:

* Outlook
* Temperature
* Humidity
* Wind

The target variable is:

* `Play` — Yes / No

The `day` column was removed before performing the calculations.

## What I Did

* Loaded the `Play Tennis` dataset using Pandas

* Removed the unnecessary `day` column

* Calculated the prior probabilities of `Play = Yes` and `Play = No`

* Created frequency tables using `pd.crosstab()`

* Calculated conditional probabilities for:

  * Outlook
  * Temperature
  * Humidity
  * Wind

* Applied the **Naive Bayes formula manually**

* Calculated the probability for:

  `Outlook = Sunny, Temperature = Hot, Humidity = High, Wind = Weak`

* Compared the calculated probabilities for `Yes` and `No`

## Libraries Used

* Python
* NumPy
* Pandas

## Main Concepts

* Naive Bayes Classification
* Prior Probability
* Conditional Probability
* Bayes' Theorem
* Categorical Data
* Probability Calculation
