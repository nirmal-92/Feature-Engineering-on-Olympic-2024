# Feature Engineering on Olympic 2024 Dataset and Future Medal Prediction

# Project Overview
This project focuses on analyzing and predicting the performance of countries in the Olympic Games, specifically using the medal list from the 2024 Olympics. The goal is to perform feature engineering on the dataset to derive meaningful insights and build a predictive model to estimate the total medals that countries might win in future Olympics, like the 2028 Games.

The project utilizes the MERN stack for data management and processing, with a primary focus on Python for data analysis and Machine Learning for predictions.

# Dataset Information
The dataset used for this project contains the following columns:

country: Name of the country
country_code: ISO code for the country
region: Geographical region of the country
gold: Number of gold medals won
silver: Number of silver medals won
bronze: Number of bronze medals won
total: Total number of medals won
gdp: Gross Domestic Product of the country
gdp_year: Year of GDP record
population: Population of the country

# Feature Engineering
In this project, various feature engineering techniques were applied to enhance the predictive power of the dataset:

# Missing Value Imputation:

GDP: Filled with the median value.
Population: Filled with the mean value.
Region: Filled with 'Unknown' for missing entries.
New Feature Creation:

gdp_per_capita: Calculated as gdp / population.
medals_per_capita: Calculated as total / population.
weighted_medal_score: Calculated using a weighted sum of medals, i.e., gold * 3 + silver * 2 + bronze.
One-Hot Encoding:

Encoded categorical variables (like region) using one-hot encoding.
Model Training and Evaluation
The dataset was split into training (70%) and testing (30%) sets.
A Random Forest Regressor was used to predict the total medal count for each country.
Feature Scaling was applied using StandardScaler for improved model performance.
Model Evaluation Metrics:
R² Score: Indicates the proportion of the variance in the dependent variable that is predictable from the independent variables.
Mean Absolute Error (MAE): Measures the average magnitude of errors in a set of predictions, without considering their direction.
Root Mean Squared Error (RMSE): Measures the square root of the average of squared differences between prediction and actual observation.
Prediction for Future Olympics (2028)
Using the trained model, predictions were made for India's performance in the 2028 Olympics. The model considered India's projected GDP, population, and historical medal performance.

# Thank You