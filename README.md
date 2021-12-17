# Predicting-Graduate-Admissions-using-ML
Dataset link : https://www.kaggle.com/adepvenugopal/predicting-graduate-admissions-using-ml/data

# Graduate Admission Analysis for UCLA
Introduction
Objective
400 applicants have been surveyed as potential students for UCLA. The university weighs certain aspects of a student's education to determine their acceptance.

The objective is to explore what kind of data is provided, determine the most important factors that contribute to a student's chance of admission, and select the most accurate model to predict the probability of admission.

Data Description
The dataset contains information about a student's:

- GRE Score
 - TOEFL Score
- University Ratings
- Statement of Purpose Score
- Letter of Recomendation Score
- CGPA
- Whether the Student Has Done Any Research
- Chance of Admission (What We're Trying to Predict)
- Importing Libraries and Data
- Importing libraries and setting the default style in Seaborn.

Machine Learning 
Now we'll implement machine learning algorithms to predict the chance of admission. We'll use multiple techniques and eventually select the method with the best score.

# PROCEDURE

Reading the csv file into pandas dataframe

 We also checked the number of rows and columns in our dataframe using the shape method.
 
 

Selecting the Best Algorithm
Multiple Linear Regression
Polynomial Regression
Decision Trees 
It seems that Multiple Linear Regression is the most accurate of the 3 methods and will be used to predict the future applicant's chances of admission and CGPA is the most important parameters that affect the chance of admission .
