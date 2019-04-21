## Information

Title: Bike Sharing Demand

Website: https://www.kaggle.com/c/bike-sharing-demand

Purpose:
- *Here's the backstory*: Bike sharing systems are a means of renting bicycles where the process of obtaining membership, rental, and bike return is automated via a network of kiosk locations throughout a city. Using these systems, people are able rent a bike from a one location and return it to a different place on an as-needed basis. Currently, there are over 500 bike-sharing programs around the world.
- Hence, we are responsible for predicting how many bikes will be demanded on the 20th for each of the month in the dataset. The training set is the first 19 days.

Scoring Metric: RMSLE
- Square_Root[1/n[Summation[(log(p + 1) - (log(a + 1))^2)]]]
  - Link: https://www.kaggle.com/c/bike-sharing-demand#evaluation
- RMSLE is usually used when you don't want to penalize huge differences in the predicted and the actual values when both predicted and true values are huge numbers.
  1. If both predicted and actual values are small: RMSE and RMSLE is same.
  2. If either predicted or the actual value is big: RMSE > RMSLE
  3. If both predicted and actual values are big: RMSE > RMSLE (RMSLE becomes almost negligible)

MyBinder Jupyter Interactive Notebooks:
  - `00_DateNotebook.ipynb`: Provides an overview of the the finding/insights during the project.
  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/alexguanga/bike-sharing-demand/master?filepath=00_DateNotebook.ipynb)
  - `01_DateNotebook.ipynb`: An All-In notebook that contains visualization, analysis, and modeling.
  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/alexguanga/bike-sharing-demand/master?filepath=01_DateNotebook.ipynb)
