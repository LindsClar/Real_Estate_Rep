# Capstone Two - Real Estate Predictions in California

Thought the process of exploring the data I had to make a few changes and pivot the data to be useful for my future modeling of the data later on. Below, you’ll see that I used .melt to take the data frame from a wide format to a long format. This made it easier for me to form the columns to graph it later and organize the dates for times series later on. 

Initially, I explored modeling with Linear Regression and decided to enhance its performance by incorporating hyperparameter tuning. Specifically, I evaluated various regularization techniques, including Ridge Regression, Lasso Regression, and Elastic Net.
After careful consideration, I chose to focus on Lasso Regression for hyperparameter tuning within the Linear Regression framework. However, the results were not promising. The modeling outcomes and associated error rates indicated suboptimal performance, suggesting potential issues with either the approach or the data itself.

In comparison to ARIMA, Random Forest, and XGBoost, Linear Regression emerged as the best modeling approach. I assessed each model’s fit by comparing actual values with predicted values, and Linear Regression demonstrated the best overall fit. 
Using Linear Regression, we observed a gradual increase in property values in San Diego. This suggests that purchasing property in San Diego would be a sound investment. Over time, homebuyers or investors are unlikely to lose equity and may see property gains.
This analysis is based solely on property values as a univariate time series. It considers only the value of a single home over a six-year period in San Diego and does not incorporate additional variables.

# Table of Contents
	1. Loading the Data
	2. Evaluating and Organizing the Data
	3. Splitting the Data
	4. Modeling
		a. Linear Regression
			- param_grid  in grid_search
			- Lasso	
		b. ARIMA
			- parameter_combinations
			- Calculated and compared predictive values to actual values
		c. Random Forest
			- param_grid in grid_search 
			- RandomForestRegressor
		d. XGBoost
			- param_grid in grid_search
			- XGBRegressor
	5. Comparing the Models
	6. Conclusion
# Future Analysis Possibilities 

To expand this analysis in the future, I would include other variables to assess their impact on property values in San Diego over the same six-year period. For instance, I would analyze how factors such as natural disasters (landslides, floods, and earthquakes) influence property values. Additionally, I would examine the effects of the political climate, including Mello-Roos parameters, COVID-19 restrictions, and permit requirements that affect housing inventory.
This analysis, based solely on home values, serves as the foundation for more comprehensive studies to evaluate the stability and volatility of the San Diego property market under various conditions.

