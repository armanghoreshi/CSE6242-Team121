****************************************************************************************
*   Remote Work & Housing Price Analysis                                               *
*   Team 121 - Arman Ghoreshi, Brett Boonie, Josh Harasaki, Jinny Kwon, Jingang Piao   *
****************************************************************************************


------------------------------------------------
|                 DESCRIPTION                 |
------------------------------------------------
This repository contains the code, data, and visualizations for analyzing the impact of remote work on U.S. real estate
markets, using regression models and interactive maps to identify high-growth counties and trends for real estate development.
The project is consist of multiple Jupyter Notebooks for data cleaning, data transformation, and predictions. The small
datasets are available in the repo but the bigger datasets are linked for download. At last the results from these Jupyter
Notebooks are fed into Tableau for an interactive visualizations.

Please find the description of each of the Jupyter Notebooks here:

1. County Labeling And Adjacency.ipynb
This notebook uses population and housing density to determine a metro county per state. Then it uses county adjacency data
to find which counties are neighbours to the metro county up to 5 levels using a DFS algorithm treating counties as nodes and
adjacency as edges.

2. clean_home_price.ipynb
This notebook performs data cleanup and transformation on the Zillow hous price index dataset to make it ready for blending
it with other datasources.

3. data_fetch_preprocess_Fred.ipynb
Fetch data from fred.stlouisfed.org API and the cleaning process for using in prediction models

4. Modeling-v4.ipynb
This notebook integrates and processes data from multiple sources performing transformations and cleaning to prepare 
the final dataset for regression modeling and time series analysis. It includes the construction of regression models,
evaluation of their performance using MSE, and detailed analysis of the results.
After finding the best model, we use that to predict the December 2024 real estate prices per county.

5. linear_regression_ARIMA_ARIMAX.ipynb
This notebook uses the same data inputs as #4 but uses ARIMA and ARIMAX for timeseries analysis.


The final tableau dashboard is published in Tableau Public:
https://public.tableau.com/app/profile/arman.ghoreshi6341/viz/RemoteWorkHousingPriceAnalysis/RemoteWorkHousePriceAnalysis


------------------------------------------------
|                INSTALLATION                 |
------------------------------------------------

run this command to install all the libraries:

pip install -r requirements.txt

------------------------------------------------
|                  EXECUTION                  |
------------------------------------------------

1. Run "clean_home_price.ipynb" and "County Labeling And Adjacency.ipynb"
2. Run "data_fetch_preprocess_Fred.ipynb"
3. Run "Modeling-v4.ipynb" and "linear_regression_ARIMA_ARIMAX.ipynb"
4. Open the tableau file "Tableau/Remote Work & Housing Price Analysis.twb"
5. Go to the data tab from the bottom left
6. Click "Refresh" in the top right
7. Click on any of the sheets in the bottom nav bar
8. Use the dashboard offline or publish it to Tableau Public