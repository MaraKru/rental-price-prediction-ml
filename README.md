# Machine Learning: Apartment Rental Price Prediction

## About the Project

A study project in Machine Learning where I built models to predict apartment rental prices. The project covers the full data workflow: from initial data analysis to building and comparing models.


### The Task

Predict an apartment's rental price based on listing features:

* Number of bathrooms (bathrooms)
* Number of bedrooms (bedrooms)
* Tenant interest level (interest_level)

Dataset: Kaggle - Two Sigma Connect (Rental Listing Inquiries)
(https://www.kaggle.com/competitions/two-sigma-connect-rental-listing-inquiries/data)


### Getting Started

Unzip the provided archives: test.zip and train.zip


### What I did

1. Initial Data Analysis
- Explored data structure
- Identified the target variable (price)
- Analyzed price distribution and detected outliers
- Removed extreme values (1st and 99th percentiles)

2. Statistical Analysis
- Created price distribution histograms
- Built a boxplot to visualize outliers
- Encoded categorical variable interest_level
- Analyzed correlations between features

3. Interesting Findings
- Strong correlation between price and number of bathrooms (0.67)
- Moderate correlation with number of bedrooms (0.55)
- Inverse relationship: higher tenant interest correlates with lower prices (-0.2)

4. Model Building
Compared four approaches: Decision Tree, Linear Regression, Naive (median), and Naive (mean). Calculated MAE and RMSE. Decision Tree performed best on both metrics.


### Technical Stack

* Python 3 + Jupyter Notebook
* Libraries: pandas, numpy, matplotlib, seaborn
* ML libraries: scikit-learn (LinearRegression, DecisionTreeRegressor)
* Metrics: MAE (Mean Absolute Error), RMSE (Root Mean Squared Error)


### What I Learned

- Working with real-world Kaggle data
- Data preprocessing (handling outliers, encoding categories)
- Building and evaluating ML models
- Interpreting performance metrics (MAE, RMSE)
- Data visualization (histograms, scatter plots, heatmaps)


### Key Insights

* Relatively simple models can perform well: Decision Tree outperformed linear regression
* Data quality is crucial: removing outliers significantly improved results
* Not all features are equally useful: number of bathrooms was more important than bedrooms
* Baseline models matter: naive models helped set a minimum performance benchmark
