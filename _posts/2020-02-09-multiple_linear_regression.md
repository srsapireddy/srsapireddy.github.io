---
title: "Machine Learning Project: Multiple Linear Regression"
date: 2020-02-08
tags: [Machine learning, data science, Multiple Linear]
header:
    image: "/images/multiple_regression/multiple_regression.png"
excerpt: "Machine Learning, Regression, Data Science"
---

# Multiple Linear Regression —
Simple linear regression : a single independent variable is used to predict the value of a dependent variable.

Equation : y=A+BX

Multiple linear regression : two or more independent variables are used to predict the value of a dependent variable. The difference between the two is the number of independent variables.

Equation : y=A+BX1+CX2+DX3

Link to my GitHub page [multiple_linear_regression](https://github.com/srsapireddy/Machine-Learning-Files-in-Python-and-R/tree/master/3.%20Multiple%20Linear%20Regression)

R code block:
```r
# Multiple Linear Regression

# Importing the dataset
dataset = read.csv('50_Startups.csv')

# Encoding categorical data
dataset$State = factor(dataset$State,
                         levels = c('New York', 'California', 'Florida'),
                         labels = c(1, 2, 3))

# Splitting the dataset into the Training set and Test set
# install.packages('caTools')
library(caTools)
set.seed(123)
split = sample.split(dataset$Profit, SplitRatio = 0.8)
training_set = subset(dataset, split == TRUE)
test_set = subset(dataset, split == FALSE)

# Feature Scaling
# Here we dont need to have feature scaling manually. This is gonna taken care by the function which we use to fit multiple
# regression to our training set
# training_set = scale(training_set)
# test_set = scale(test_set)

# Fitting Multiple Linear Regression to Training Set
# Formula -> Here the profit (dependent variable) is going to be the linear combination of the independent variables
regressor = lm(formula = Profit ~ ., data = training_set)
# Here we can see that is automatically removed the dummy variable to avoid some reduncant dependncy
# Estimate -> Coefficienct in the linear regression equation
# *** -> Significance Level of independnt variable on the independent variable
# Lower the P - value is the more the statistically significant our independent variable is going to be (generally 5% threshold)
# When p - value is between 0 and 0.1% then we have 3 stars (***)
# If p - value is between 0.1% and 1% then we have 2 stars - quite high levl of statistical significance
# If p - value is between 1% and 5% then the independent variable is still statistical significant but with a less strong effect than the first categories
# If p - value is between 5% and 10% it is in the borderline. The independent variable might have a certain level of statistical significance but not that much.
# If p - value is between 10% and 1 then there is no statistical significance. The independent variable will not have any effect on dependent variable.
summary(regressor) # Here the Profit is mainly governed by the R & D Spend. Thus we can turn this into a Multiple Linear Regression.

# Predicting the Test Results
y_pred = predict(regressor, newdata = test_set)

# Building the Optimal Model using Backward Elimination
regressor = lm(formula = Profit ~ R.D.Spend + Administration + Marketing.Spend + State, data = training_set)
summary(regressor)

regressor = lm(formula = Profit ~ R.D.Spend + Administration + Marketing.Spend, data = training_set)
summary(regressor)

regressor = lm(formula = Profit ~ R.D.Spend + Marketing.Spend, data = training_set)
# Here we get a dot at endof Marketing Spendp - value because of the jump in p - value
summary(regressor)

regressor = lm(formula = Profit ~ R.D.Spend, data = training_set)
summary(regressor)
```

## Applications of Multiple Linear Regression
In the social and natural sciences multiple regression procedures are very widely used in research. In general, multiple regression allows the researcher to ask (and hopefully answer) the general question "what is the best predictor of ...". For example, educational researchers might want to learn what are the best predictors of success in high-school. Psychologists may want to determine which personality variable best predicts social adjustment. Sociologists may want to find out which of the multiple social indicators best predict whether or not a new immigrant group will adapt and be absorbed into society.
