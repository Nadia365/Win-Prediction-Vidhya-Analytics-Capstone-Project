# Win-Prediction-Vidhya-Analytics-Capstone-Project 
# Win-Prediction
In this project, we will analyze and predict the win possibilities of deals/projects for an IT consulting company and see how the possibility of winning a deal is impacted by other variables. This will enable the IT consulting company to manage the effort required to win a deal to meet the growth targets.  

# Objectives 
Objective 1: Predictive Analytics - Build a ML model to predict the probability of win/loss for bidding activities for a potential client.
Objective 2: Prescriptive Analytics – Identify variable/s that are most likely to help in converting an opportunity into a win. 

# Project Overview
  - Created a ML model that  helped data scientist in TI consulting comapny to to predict the probability of win/loss for bidding activities for a potential client.
  - Optimized Random ForestForest CLassifier  using Randomized Search to reach the best model. 
   
# Tools  
Python v 3

# Libraries used:

pandas
numpy
matplotlib.pyplot
sklearn
# Data Cleaning 
 -Remove duplicated features  
- Add missed values in Client Category to the ‘Others’ category 
- One hot encoding for all categorical variables except for  VP names
- Manager Name was identified as highly cardinalso, decided not to go with one hot encoding.
- Frequency Encoding performed Manager Names ranked on the basis of their frequency of occurrence.
- Removed Outliers by capping the extremes to 3rd inter Quartile. 
- Decompose the Date data into year, month , day, day of week and quarter

# EDA 
- I looked at the distributions of the data and the value counts for the various categorical variables. 
- Deal Cost is right skewed and contains many outliers 

# Model Building 
 I also split the data into train and tests sets with a test size of 0%.

I different models and evaluated them using accuracy. 
Random Forest – With the sparsity associated with the data, I thought that this would be a good fit. it is robust to outliers and prone to overfitting plus gives the best accruacy of all tested models

# Model Performance  
 The Random Forest model far outperformed the other approaches on the test and validation sets. 
Accuracy: 78% 
Accuracy after tuning: 81% 
