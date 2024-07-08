# Car-Price-Prediction

This project aims to predict the price of cars using various features of the car. The dataset used contains information about different car models, including specifications such as engine size, horsepower, and other attributes. The analysis and prediction are carried out using Python and several data science libraries.

## Table of Contents
* **Installation**
* **Data Preprocessing**
* **Exploratory Data Analysis (EDA)**
* **Feature Engineering**
* **Model Building**
* **Evaluation**
* **Conclusion**

## Installation
To run the notebook, you need to have Python installed along with the following libraries:
* numpy
* pandas
* matplotlib
* seaborn
* scikit-learn
You can install these libraries using pip:
![image](https://github.com/Ashar18/Car-Price-Prediction/assets/64865488/0617c80b-ac10-4a74-a541-17be0eedfc89)

## Data Preprocessing
1. Loading the data: The dataset is loaded using 'pandas.read_csv()' function.

2. Splitting company name from CarName column: The 'CarName' column is split to extract the company name and a new column 'CompanyName' is created.

3. Standardizing company names: The 'company' names are converted to lowercase and some misspelled names are corrected.

## Exploratory Data Analysis (EDA)
Various plots are generated to understand the distribution and relationships of the data:

* **Price distribution and spread**: Distribution plot and box plot of car prices.
* **Histograms**: Frequency distribution of different categorical features like CompanyName, fueltype, carbody, etc.
* **Box plots**: Relationship between categorical features and car prices.

## Feature Engineering
1. **Creating new features**: A new feature fueleconomy is created as a weighted average of citympg and highwaympg.

2. **One-hot encoding**: Categorical variables are converted to dummy variables.

3. **Selecting features**: Features with a correlation greater than 0.5 with the target variable price are selected.

## Model Building
1. **Data scaling**: Features are scaled using MinMaxScaler.

2. **Train-test split**: The dataset is split into training and testing sets.

3. **Model training**: A linear regression model is trained on the training set.

## Evaluation
* The model is evaluated using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

* The R-squared scores for training and testing sets are also computed.

## Conclusion
The project demonstrates the process of predicting car prices using linear regression. The analysis includes data preprocessing, feature engineering, model building, and evaluation. The results provide insights into the factors affecting car prices and the performance of the prediction model. The model achieves an accuracy of 85% on the training data and 81% on the test data.
