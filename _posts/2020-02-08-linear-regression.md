---
title: "Machine Learning Project: Linear Regression"
date: 2020-02-08
tags: [Machine learning, data science, regression]
header:
    image: "/images/linear_regression/linear_regression.png"
excerpt: "Machine Learning, Regression, Data Science"
---

# Regression — Predict continuous value of a given data point

Link to my GitHub page [linear_regression](https://github.com/srsapireddy/Machine-Learning-Files-in-Python-and-R/tree/master/Regression/2.%20Simple%20Linear%20Regression)

Python code block:
```python

# Importing the libraries
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd

# Importing the dataset
dataset = pd.read_csv('Salary_Data.csv')
#Creating matrix of features of independent variable x (30,1) and the vector y of dependent variable (30,)
X = dataset.iloc[:, :-1].values
y = dataset.iloc[:, 1].values

# Splitting the dataset into the Training set and Test set
from sklearn.cross_validation import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 1/3, random_state = 0)

#*** Here Python will take care of Feature Scaling here The libraries are gonna take of that ***
# Feature Scaling
"""from sklearn.preprocessing import StandardScaler
sc_X = StandardScaler()
X_train = sc_X.fit_transform(X_train)
X_test = sc_X.transform(X_test)
sc_y = StandardScaler()
y_train = sc_y.fit_transform(y_train)"""

# Fitting simple linear regression model to training set
# Here the object will be simple linear regressor because it is the regressor we are going to fit to the training set
# To fit to the training set we will use a method because linear regression class has several methods and one of the method is the fit method is just like a tool of function
# Importing linear regression class
from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
# Fitting -> Our code will already have learned the correlation of the training set to learn how to predict the y_train
regressor.fit(X_train, y_train)

# Predicting the Test Set Results
# Here we create a vector of predctive values -> We will create a vector of predctive values of the Test Set salaries and we will put all these predicted salaries into a single vector y_pred
# y_pred -> Vector of predicted dependent variables
y_pred = regressor.predict(X_test)

# Visualizing the Training Set
plt.scatter(X_train, y_train, color = 'red')
# Here we are gonna compare the real salaries and the predicted salaries based on the same observations. That is the observations of the training set
plt.plot(X_train, regressor.predict(X_train), color = 'blue')
plt.title('Salary vs Experience (Training Set)')
plt.xlabel('Years of Experience')
plt.ylabel('Salary')
plt.show()

# Visualizing the Test Set
plt.scatter(X_test, y_test, color = 'red')
# Here we are gonna compare the real salaries and the predicted salaries based on the same observations. That is the observations of the test set
plt.plot(X_train, regressor.predict(X_train), color = 'blue')
plt.title('Salary vs Experience (Test Set)')
plt.xlabel('Years of Experience')
plt.ylabel('Salary')
plt.show()
```

R code block:
```r
# Simple Linear Regression

# Importing the Dataset
dataset = read.csv('Salary_Data.csv')
# dataset = dataset[, 2:3]

# Splitting the data into Training Set and Test Set
library(caTools)
set.seed(123)
split = sample.split(dataset$Salary, SplitRatio = 2/3)
training_set = subset(dataset, split == TRUE)
test_set = subset(dataset, split == FALSE)

# Feature Scaling -> R gonna take care of it
# training_set[, 2:3] = scale(training_set[, 2:3])
# test_set[, 2:3] = scale(test_set[, 2:3])

# Fitting Simple Linear Regression to our Training Set
# Here we are using lm function
# formula -> dependeent variaBle expressed as a linear combination of independent variable
regressor = lm(formula = Salary ~ YearsExperience, data = training_set)
# summary(regressor)
# It tells about statistical significance of the cofficients
# The 3 stars at the end tells that the independent variable and dependent variable are highly significant (strong linear relationship)
# Lower the P value is the high the significance will be
# P value - When we are below 5 % the independent variable will be highly significant
# Multiple R - squared and Adjusted R - squared tells about the evulating the model

# Predicting the Test Set results
y_pred = predict(regressor, newdata = test_set)

# Visualizing Training Set Results
# install.packages('ggplot2')
library(ggplot2)
ggplot() +
  geom_point(aes(x = training_set$YearsExperience, y = training_set$Salary), colour = 'red') +
  geom_line(aes(x = training_set$YearsExperience, y = predict(regressor, newdata = training_set)), colour = 'blue') +
  ggtitle('Years of Experience vs Salary (Training Set)') +
  xlab('Years of Experience') +
  ylab('Salary')

# Visualizing Test Set Results
# install.packages('ggplot2')
library(ggplot2)
ggplot() +
  geom_point(aes(x = test_set$YearsExperience, y = test_set$Salary), colour = 'red') +
  geom_line(aes(x = training_set$YearsExperience, y = predict(regressor, newdata = training_set)), colour = 'blue') +
  ggtitle('Years of Experience vs Salary (Training Set)') +
  xlab('Years of Experience') +
  ylab('Salary')
# As our regressor is already trained on the Training Set there is no need to change the geom_line. We obtain the same Simple
# Linear Regression Line whether we keep training_set or the test_set here

```

## H2 Heading

### H3 Heading

Here's some basic text.

And here's some *italics*

Here's some **bold** text.

What about a [link](https://github.com/dataoptimal?)

Here's a bulleted list:
* First item
+ Second item
- third item

Here's a numbered list:
1. First
2. Second
3. Third

Here's some inline code `x+y`.

Here's an image:
<img src="{{ site.url }}{{ site.baseurl }}/images/perceptron/linsep.jpg" alt="linearly separable data">