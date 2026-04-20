# medical-insurance-cost-prediction
This is a machine learning project that aims to be able to predict the medical insurance charges paid annually by individuals based on their demographics and lifestyle.

# Summary
Over the years, there has been a rise in healthcare costs. This rise (and in particular the health insurance) has made it essential for us to look into the factors that contribute the most to medical expenses. This is what this exercise has tried to address. In this project, I sampled/tested three different regression models and built one (based on the one that gave the best results) that forecasts the cost of annual medical insurance cost using features given in the data: age, sex, BMI, children, smoker and region. The project explores cost drivers and visualises how an individual's health behaviour impact their insurance costs.

# Objectives
- Practice end-to-end data science workflow
- Identify key drivers of the medical insurance cost
- Test different regression models, understand how they function and choose the best
- Predict the annual insurance cost using regression model

# Dataset 
- Name of Dataset: Medcical Cost Personal Dataset
- Rows: 1,338 samples
- Features: age, sex, BMI, children, smoker, region
- Target: charges

Column    |  Type    |  Description
----------|----------|-------------------------------------------
age       |  int     |  age in years of primary beneficiary
sex       |  object  |  insurance contractor gender (male/female)
bmi       |  float   |  body mass index
smoker    |  object  |  yes/no
children  |  int     |  number of children covered by health insurance
region    |  object  |  beneficiary's residential area in the US (NE, SE, SW, NW)
charges   |  float   |  annual medical insurance cost

# Workflow
1. EDA (Exploratory Data Analysis)
   - Summary of data
   - Examine outliers, missing and duplicate data
   - Examine the distribution of insurance charges
   - Check relationships
2. Data Preprocessing
   - Define features
   - Train/test split
   - Define metrics
3. Modelling
   - Models tested:
     - Linear regression model
     - ridge regression model
     - RandomForestRegressor model
4. Model evaluation
   - MAE (Mean Absolute Error)
   - RMSE (Root Mean Squared Error)
   - R2 (R Squared Error)

# Graphs
Distribution of insurance charges
![Distribution](Images/dist_insurance_output.png) 



# Model performance table
Model                    |    MAE       |    RMSE      |    R2    |
-------------------------|--------------|--------------|----------|
linear regression        | 4186.508898  | 5799.587091  | 0.783346 |
ridge regression         | 4198.141005  | 5803.084710  | 0.783085 |
RandomForestRegressor    | 2470.926342  | 4537.517293  | 0.867380 |

The random forest regressor model produced the lower error and was used to build the predictive model. 

# Insights
- Smoking dramatically increases the medical insurance cost when compared to the other features.
- Age and BMI contribute to higher insurance costs.
- Sex and region have minimal impact.
