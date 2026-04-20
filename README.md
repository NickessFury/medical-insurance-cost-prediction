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

