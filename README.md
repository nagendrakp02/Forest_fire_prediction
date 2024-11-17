
# Forest Fire Prediction


## A brief description of what this project is all about.

Forest Fire Prediction is a Supervised Machine learning problem statements.
Using Regression  is build that detected future fires based on certain Weather report.

A framework is created using **Flask** and deployed on **Elastic Beanstalk**

## Library Used in this Project 

**Data Pre-Processing**

- **Numpy**, **Pandas**, **Matplotlib**, **Seaborn**

**Model Building**

- **Sklearn**, **statsmodels**

**Hyperparameter Tuning**

## Introduction

**Algerian Forest Fires**


**Data set Available at:** [link text]('models/algalgeria_cleaned.csv')

***Data Set Information:***

- The dataset includes 244 instances that regroup a data of two regions of **Algeria**,namely the 
 - **Bejaia region** located in the **northeast of Algeria** and the **Sidi Bel-abbes region** located in the **northwest of Algeria**.

- 122 instances for each region.

- The period from June 2012 to September 2012.
- The dataset includes 11 attribues and 1 output attribue (class)
- The 244 instances have been classified into **fire** (138 classes) and **not fire** (106 classes) classes.

**Attribute Information:**

**1. Date :** (DD/MM/YYYY) Day, month ('june' to 'september'), year (2012)

**Weather data observations**

**2. Temp :** temperature noon (temperature max) in Celsius degrees: 22 to 42

**3. RH :** Relative Humidity in %: 21 to 90

**4. Ws :** Wind speed in km/h: 6 to 29

**5. Rain:** total day in mm: 0 to 16.8

**FWI Components**

**6. Fine Fuel Moisture Code (FFMC) index from the FWI system:** 28.6 to 92.5

**7. Duff Moisture Code (DMC) index from the FWI system:** 1.1 to 65.9

**8. Drought Code (DC) index from the FWI system:** 7 to 220.4

**9. Initial Spread Index (ISI) index from the FWI system:** 0 to 18.5

**10. Buildup Index (BUI) index from the FWI system:** 1.1 to 68

**11. Fire Weather Index (FWI) Index:** 0 to 31.1

**12. Classes:** two classes, namely **Fire** and **not Fire**

# Steps 

1. Data Collection
2. Data Pre-Processing
3. Exploratory Data Analysis
4. Feature Engineering
5. Feature Selection
6. Model Building
7. Model Selection
8. Hyperparameter Tuning
9. Flask framework
10. Model deployment 

## Model Building

**Regression** 

- For regression analysis **FWI(Fire weather Index)** considered as dependent feature because it highly correlated with classes variable with more than 90% correlation.

**Model Used:** 

1. Linear regression
2. Lasso Regression
3. Ridge Regression

**Classification**

- For Classification **Classes** is dependent feature which is a **Binary Classification(fire, not fire)**

## Model Selection

HyperParameter Tuning performed using **RidgeCV** for the model which performed best for both Regression and Classification.

- For Regression **r2_score** metrics is used to select best model.

- For Classification **Stratified Kfold Cross-Validation** metrics is used.
- The best Mean CV Accuracy Model is used for Model Deployment.

## Model Deployment

**Flask**
- framework is created using Flask.


