## `Sales Price Forecasting`

**AIM**

- The objective is to predict future daily sales for thousands of stores based on historical data. Predictive models attempt at forecasting future sales based on historical data while taking into account seasonality effects, demand, holidays, promotions, and competition. For instance black Friday sales go crazy so the model has to take into effect all these scenarios.

**Methodology**

- `Exploratory Data Analysis`

  EDA is the process of analyzing the data set to understand its characteristics. In this case:

  - Number of closed, open stores, competition distance etc
  - Are they any NAN?
  - Find outliers
  - Check for duplicate values
  - Correlations

- `Visualization to answer few questions`
  - Further EDA by raising a few questions on the dataset and finding out answers for the same using various visualization and data manipulation technique. This helps in getting an in-depth understanding about the data set.
- `Imputation`

  Filling of missing values in appropriate ways so that we don't lose much data. The detected missing values are filled appropriately.

- `Modeling with Facebook Prophet`

  Facebook prophet is an open source software released by Facebook's core Data Science team. Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality plus holiday effects. It works best with time series that has seasonality effects and several seasons of historical data.

  - Additive regression model take the form

  $$y(t) =g(t) + s(t) + h(t) + \epsilon(t)$$

       - $g(t)$ : piecewise linear or logistic growth curve for modeling non-periodic changes in time series.
       - $s(t)$ : periodic changes (e.g weekly/yearly seasonality)
       - $h(t)$ : effects of holidays (user provided) with irregular schedules
       - $\epsilon(t)$ : error term accounts for any unusual changes not accommodated by the model.

* Prophet works with missing data and outliers, very easy to tune model hyperparameters like changepoints.
