# CSE6242-Team121
Team 121 - Data Visualization &amp; Analytics

********************************************************************FRED DATA PROCESS*********************************************************************************************************************************************************************************************************************************************
Launch data_fetch_preprocess_fred.ipynb 
and run each cells to fetch demographic and economic data from FRED website and run the preprocessing of the data by adding county FIPS code.
Fred data fetch and preprocess:
./data/fips.txt -- used to create state and county fips code,output file is countyname.csv

below are unprocessed files under ./data/ after fetch from FRED website:
1 unemployment_by_county.csv - output of process file is modified_unemployment_per_county.csv
2 median_income_by_county.csv - output of process file is modified_median_income_per_county.csv
3 homeowner_by_county.csv - output of process file is modified_homeowner_per_county.csv
4 income_inequality_by_county.csv - output of process file is modified_income_inequality_per_county.csv
5 meancommute_by_county.csv - output of process file is modified_mean_commutetime_per_county.csv
6 poppoverty_by_county.csv - output of process file is modified_population_under_poverty_per_county.csv
7 respop_by_county.csv - output of process file is modified_resident_population_per_county.csv
8 gdp_by_county - output of process file is modified_gdp_per_county.csv
9 totallist_by_county.csv - output of process file is modified_totallisting_per_county.csv
********************************************************************FRED DATA PROCESS*********************************************************************************************************************************************************************************************************************************************
********************************************************************Linear regression, ARIMA,ARIMAX modeling**********************************************************************************************************************************************************************************************************************
Before running codes below, you need to download the dataset from this link :https://drive.google.com/file/d/1sVQymlc-lKv1_Ghf0MYZk0QdRpdRRZim/view?usp=drive_link
Launch linear_regression_ARIMA_ARIMAX.ipynb and run each cells to create linear regression, ARIMA, ARIMAX based models on Home Prices for each county and also plots for San Francisco county as an example of home price prediction. Then it calculates the RMSE for each algorithm for all the counties and take average of them to represent the average RMSE for 3 algorithms to compare their pros and cons.




********************************************************************Linear regression, ARIMA,ARIMAX modeling**********************************************************************************************************************************************************************************************************************


