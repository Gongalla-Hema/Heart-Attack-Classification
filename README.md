
# Heart Attack Classification

Use machine learning to create a model that predicts whether a person will suffer from Heart failure.

## Acknowledgements

 - [Dataset on Kaggle](https://www.kaggle.com/datasets/andrewmvd/heart-failure-clinical-data?datasetId=727551&sortBy=voteCount)
 - [Data Science Methodology](https://www.coursera.org/learn/data-science-methodology)

## Project Pipeline

- Business Understanding
- Analytical Approach
- Data requirements
- Data collection
- Data Understanding
- Data Preparation
- Modeling
- Evaluation


## Libraries used

- Numpy
- Pandas
- Seaborn
- Sickit-Learn 

```bash
  pip install numpy, pandas, seaborn, sklearn
```
    

## Business Understanding

Cardiovascular diseases (CVDs) are the number 1 cause of death globally, taking an estimated 17.9 million lives each year, which accounts for 31% of all deaths worldwide. Four out of 5CVD deaths are due to heart attacks and strokes, and one-third of these deaths occur prematurely in people under 70 years of age. Heart failure is a common event caused by CVDs and this dataset contains 11 features that can be used to predict a possible heart disease.

The challenge here is - Given a person's information, how can we predict whether he/she will suffer from Heart Failure

## Analytical Approach

Our target variable is categorical and hence we need classification models for this task.


## Data requirements

We would require onboard passengers information which might include name, age, fare, gender, class.


## Data collection

We are given two datasets both of which are CSV files, one for training our model named as train.csv and the other test.csv to test if our model can make accurate prediction. 

## Data Understanding

This step is part of Exploratory Data Analysis

There are 918 observations in the training dataset with each having 12 columns. 11 of them are predictor variables and 1 being target variable.

There are few different types of variables available.

- Age: age of the patient [years]
- Sex: sex of the patient [M: Male, F: Female]
- ChestPainType: chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
- RestingBP: resting blood pressure [mm Hg]
- Cholesterol: serum cholesterol [mm/dl]
- FastingBS: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
- RestingECG: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
- MaxHR: maximum heart rate achieved [Numeric value between 60 and 202]
- ExerciseAngina: exercise-induced angina [Y: Yes, N: No]
- Oldpeak: oldpeak = ST [Numeric value measured in depression]
- ST_Slope: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
- HeartDisease: output class [1: heart disease, 0: Normal]


## Data Preparation / Feature Engineering
After closely looking into the dataset, variables types, values, amount of missing values present, I have decided to
- Impute the missing values
- Turn categorical values into an ordinal feature

I also performed some feature engineering as there are few categorical variables present.

Also standardization was performed for numerical values.

## Modeling
Models trained
- Logistic Regression
- k-Nearest Neighbors
- Support Vector Machines
- Naive Bayes classifier
- Decision Tree
- Random Forest

## Evaluation
Decision Tree and Random Forest achieved the maximum accuracy of 88%. 
