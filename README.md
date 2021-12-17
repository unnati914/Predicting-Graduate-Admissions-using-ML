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
 
  We also checked the number of rows and columns in our dataframe using the shape method.
  
  It's always important to know the correlation between each element in a data set in order to uderstand the degree of association between two variables. Thus, we also checked the correlation between the elements in our data set using corr().
 
 From the above matrix we can see that there is a strong positive correlation between GRE score and TOEFL score, GRE score and CGPA, GRE score and Chance of Admit, TOEFL score and CGPA, TOEFL score and Chance of Admit and lastly; CGPA and Chance of Admit.
 
 ### Identify and handle missing value
 
  Based on the summary , none of the columns containing missing data
  
  As seen from the box plots there seem to be outliers in LOR and Chance of Admit Values. We used Interquartile range rule for outliers to remove outliers.
  
 ## Hypothesis 
 
 Hypothesis 1: How important are GRE, TOEFL scores and CGPA important in getting an admit?
 
 Selecting required features for analysis
 
 Visualizing each attribute wrt Chance of admit using histogram & scatterplot.
 
 We used LinearRegression() function to treat polynomial regression as linear regression so that we could analyze this model easily. 
 
 ## Result 
 
 As we can see from the above dataframe all three models are good models to predict the chance of admit. But the best model amongst the 3 models is Multiple linear regression model since it has lowest mean absolute error as well as lowest mean squared error and the highest R2-Score. Polynomial regression has no mean squared error but it has higher mean absolute error and lower R2-Score when compared to multiple linear regression model. In case of regression tree it has higher mean absolute error and higher mean squared error than multiple linear regression and polynomial regression. It also has lowest R2-Score, hence it is not the best model when compared with other two. Thus, after comparing all three models we concluded that multiple linear regression is the best model. Also, we found out that GRE,TOEFL Scores and CGPA are really important variables in obtaining an admit from the university as higher GRE/TOEFL scores and higher CGPA would lead to greater chances of getting admit from a university.
 
 ## Hypothesis 2
 
 Hypothesis 2: Does higher rating of SOP and LOR leads to greater chance of admit?
 
 As we saw from our scatter plot matrices there seem to be a little or no correlation between the SOP/LOR and chance of admit. Hence, looking at our 3 models we got a very low R2-Score. The relatively high R2-score was observed for Polynomial Regression (-0.06). Polynomial regression also has lower mean absolute error and mean squared error when compared to Regression tree. Hence, amongst our three models Polynomial Regression would be the best one. But over-all it can be concluded that higher rating of SOP and LOR does not necessarily lead to higher chances of admit. Maybe SOP and LOR coupled with other variables might lead to more accurate predictions but just SOP and LOR are not ideal variables to predict the chance of obtaining an admit from the university.
 
 ## Hypothesis 3
 
 Hypothesis 3: What are the chances of getting an admit from the university considering all variables (i.e. GRE Score,TOEFL Score,University Rating, SOP, LOR, CGPA, Research)?
 
 As we can see from the  dataframe all three models are decent models to predict the chance of admit. But the best model amongst the 3 models is Multiple linear regression model since it has lowest mean absolute error as well as lowest mean squared error and the highest R2-Score. Polynomial regression has lower mean squared error and lower mean absolute error but lower R2-Score when compared to regression tree model. In case of regression tree it has higher mean absolute error and higher mean squared error than multiple linear regression. It also has lower R2-Score, hence it is not the best model when compared with linear regression model. Thus, after comparing all three models we concluded that multiple linear regression is the best model. Also, we found out that considering all variables for prediction does not lead to higher accuracy results as we got a model with better fit when we considered only GRE Score, TOEFL Score and CGPA.
 
 

Selecting the Best Algorithm
Multiple Linear Regression
Polynomial Regression
Decision Trees 
It seems that Multiple Linear Regression is the most accurate of the 3 methods and will be used to predict the future applicant's chances of admission and CGPA is the most important parameters that affect the chance of admission .
