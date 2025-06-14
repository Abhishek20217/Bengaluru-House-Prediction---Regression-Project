# Bengaluru-House-Prediction - Regression Project
## Overview
This project focuses on predicting house prices in Bengaluru using regression techniques like Linear Regression, Lasso and Decision Tree Classifier and with Hyperparameter tuning using GridSearchCV. It includes data cleaning, feature engineering, and model selection to build a reliable machine learning pipeline. The project serves as a practical example of solving real estate price prediction problems using Python and data science Algorithms.

## Dataset used
<a href= "https://github.com/Abhishek20217/Bengaluru-House-Prediction---Regression-Project/blob/main/Bengaluru_House_Data.csv"> Bengaluru House Pricing Data </a>

This dataset contains information about Bengaluru, India house pricing. It has columns such as:
1) Location - Area of the property in bengaluru.
2) Size - Number of Bedrooms (eg 2BHK, 3BHK)
3) Total_Sqft - Total Area of the property in sqft.
4) Bath - Number of Bathrooms.
5) Balcony - Number of Balconies.
6) Price - Property price in lakhs.

## Project Workflow
### Data Cleaning
* Dropped columns like 'Society', 'Availability', and 'Area_type' as they were not useful.
* Handled missing values using different Stratergies.
* Converted 'total_sqft' to numerical format as it was not in proper format.
* Extracted numerical features from textual fields ( eg. 'size' to number of bedroom)

### Feature Engineering
* Created new columns like 'BHK' and filtered out the outliers (some unrealistic prices)
* Converted categorical variables like 'Location' (after dimentionality reduction)

### Model Building
Tested different Regression Models to see which is best for house price prediction
* GridSearchCV for hyperparameter tuning.
* Linear Regression.
* Lasso Regression.
* Decision Tree Classifier.

## Result
Linear Regression performed better than Lasso Regression and Decision Tree Classifier with an accuracy of 81.9% compared to 68.7% and 72.4% for Lasso Regression and Decision Tree Classifier respectively.

![Bengaluru house price using different regression models](https://github.com/user-attachments/assets/bd91f389-aeaa-4e4f-93e6-90c76a49b532)


## Limitations
* There are other external factors like market trends and amenities which is not in the dataset so the prices may differ with these factors.
* Some features like 'Total_sqft' are inconsistently formatted and we did assumption with the data.

## Future Work
* Integrate Geospatial features using the Longitude and Latitude.
* Build a web interface to show the predictions using python flash server with the help of PyCharm or Streamlit.

## Jupyter Notebook File
<a href='https://github.com/Abhishek20217/Bengaluru-House-Prediction---Regression-Project/blob/main/Bengaluru%20House%20Prediction%20-%20Regression%20Project.ipynb'> Bengaluru House Price Prediction using Regression </a>


