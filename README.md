# Predicting Rain in Australia

## Introduction
Is it possible to predict if it will rain the following day in Australia through the implementation of different models using Python and Scikit-Learn.


## Data Exploration
- Data Preparation and Feature Selection
![image](https://user-images.githubusercontent.com/100037523/218308941-81b6482e-31f0-4a82-a4bd-db021e659ba4.png)

## Exploratory Data Analysis through Python
![image](https://user-images.githubusercontent.com/100037523/218308991-9d6a4185-7c99-40b2-b59e-577b0c9ff4d7.png) ![image](https://user-images.githubusercontent.com/100037523/218308995-ad509faa-15ec-4d4e-9a3b-35982be1d5b7.png)
![image](https://user-images.githubusercontent.com/100037523/218309104-38ae8e46-05c6-4d20-a72e-b1f4216c36e4.png)
![image](https://user-images.githubusercontent.com/100037523/218309105-b08ed8e4-10df-43ba-b24d-a24d53083474.png)
![image](https://user-images.githubusercontent.com/100037523/218309111-9859c2e6-90a5-4c4e-ba64-63774dc27b16.png)

## Data Preparation
### - Missing values
 - **__Isnull()__** is used to find the missing values in the data and these are the variables that has missing values.
  ![image](https://user-images.githubusercontent.com/100037523/218309269-d143661c-0000-489f-bcdd-2947a76c3997.png)
  
  Cloud9am & Cloud3pm has 37.7% and 40.2% missing data respectively.
  They will be removed
 
 - **__RISK_MM__** is removed
   - According to the author of the dataset. This is what he wrote himself.
    "Note: You should exclude the variable Risk-MM when training a binary classification model. Not excluding it will leak the     answers to your model and reduce its predictability. Read more about it here (https://www.kaggle.com/jsphyg/weather-     =dataset-rattle-package/discussion/78316)."
 - **__DATE__** is removed
   - not needed when I need to predict rain based on the weather/environment.
 - **__Cloud9am & Cloud3pm__** is removed
   - more than 1/4 of the data are missing.
 - **__Location__** is removed
   - I want to find if it will rain in Australia(generalized) and not in specific a location.


