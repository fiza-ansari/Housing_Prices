**PROJECT OVERVIEW:**
The dataset includes information about transactions at a coffee shop. The dataset consists of 89120 rows and 20 columns
The columns in the dataset are:
•	PROPERTY_ID
•	LOCATION_ID
•	PAGE_URL
•	PROPERTY_TYPE
•	PRICE
•	LOCATION
•	CITY
•	PROVINCE_NAME
•	LATITUDE
•	LONGITUDE
•	BATHS
•	AREA
•	PURPOSE
•	BEDROOMS
•	DATE_ADDED
•	AGENCY
•	AGENT
•	AREA TYPE
•	AREA SIZE
•	AREA CATEGORY

**OBJECTIVE:** 
Analyze a dataset of house prices to understand pricing factors, identify outliers, and develop a model for future price prediction.
Tasks:

**1.	Data Cleaning and Exploration:**	
•	**Clean the data:** _Identify and handle missing values, inconsistencies, and outliers._
•	**Explore the data:** _Analyze the distribution of house prices and other features. Identify potential relationships between features and price using visualizations (scatter plots, box plots, etc.)._
 
**2.	Feature Engineering:** 
•	_Create new features that might be relevant for price prediction (e.g., age of the house, number of bedrooms per floor)._
•	_Consider encoding categorical features (e.g., location) into numerical values suitable for modeling._
 
**3.	Outlier Analysis:** 
•	_Identify houses with significantly higher or lower prices compared to similar properties._ 
•	_Investigate the reasons for these outliers. Are there any specific features or combinations of features that contribute to the outliers?_
 
**1	A perfect positive correlation is denoted by 1.
2	A value of 0 denotes no correlation.
3	A perfect negative correlation has a value of -1.**

_**Matrix Interpretation:**_

**Self-Correlation:**
•	The diagonal elements of the matrix are all 1 because each feature is perfectly correlated with itself.
**Price Relationships:**
•	The price of a property tends to go up as the number of bathrooms, bedrooms, and total rooms increases. This is shown by the moderate positive correlations: 0.32 with bathrooms, 0.4 with bedrooms, and 0.39 with total rooms.
•	However, the size of the property in marla (a unit of area) doesn’t have much of a direct relationship with the price (correlation of 0.011), meaning the area size doesn't significantly affect the price.
Bathrooms, Bedrooms, and Total Rooms:
•	Properties with more bathrooms tend to have more rooms overall. Bathrooms are strongly correlated with total rooms (0.93) and moderately correlated with bedrooms (0.62).
•	Similarly, the total number of rooms is highly correlated with the number of bedrooms (0.86) and bathrooms (0.93), indicating that properties with more rooms typically have more bedrooms and bathrooms.
**Price Per Unit Area:**
•	The price per unit area (how much the property costs per unit of area) is somewhat related to the overall price of the property, with a moderate positive correlation of 0.4.
•	However, the price per unit area doesn’t have strong correlations with other features like bathrooms, bedrooms, total rooms, or area in marla.
**4.	Predictive Modeling:** 
•	Train a machine learning model to predict house prices based on the available features. Popular choices for this task include linear regression, random forest, or gradient boosting.
•	Evaluate the performance of the model using appropriate metrics (e.g., mean squared error, R-squared).
 

**5.	Future Price Prediction:**
•	_Use the trained model to predict future house prices based on hypothetical scenarios (e.g., what would be the price of a house with specific characteristics in a particular location?)._
 
**FINDINGS:
•	The price of a property tends to go up as the number of bathrooms, bedrooms, and total rooms increases.
•	The size of the property in marla (a unit of area) doesn’t have much of a direct relationship with the price.
•	Properties with more bathrooms tend to have more rooms overall.
•	The total number of rooms is highly correlated with the number of bedrooms and bathrooms.
•	The price per unit area is somewhat related to the overall price of the property.**

**CONCLUSION:**
The Random Forest model is the most accurate model for predicting house prices. It has the lowest MSE (114,421,988,781.18144) and the highest R-squared value (0.9991108345702634).
