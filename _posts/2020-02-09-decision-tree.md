---
title: "Machine Learning Project: Decision Tree Regression"
date: 2020-02-08
tags: [Machine learning, data science, Decision Tree]
header:
    image: "/images/decision_tree/dt1.jpg"
excerpt: "Machine Learning, Regression, Data Science"
---

# Decision Tree Regression:
Decision tree regression observes features of an object and trains a model in the structure of a tree to predict data in the future to produce meaningful continuous output. Continuous output means that the output/result is not discrete, i.e., it is not represented just by a discrete, known set of numbers or values.

Discrete output example: A weather prediction model that predicts whether or not there’ll be rain in a particular day.

Continuous output example: A profit prediction model that states the probable profit that can be generated from the sale of a product.

Link to my GitHub page [Decision_Tree_Regression](https://github.com/srsapireddy/Machine-Learning-Files-in-Python-and-R/tree/master/Regression/6.%20Decision%20Tree%20Regression)

Python code block:
```python
# Data Preprocessing
# Importing the libraries
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd

# Importing the dataset
dataset = pd.read_csv('Position_Salaries.csv')
X = dataset.iloc[:, 1:2].values
y = dataset.iloc[:, 2].values

# Splitting the dataset into the Training set and Test set
"""from sklearn.cross_validation import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.2, random_state = 0)"""

# Feature Scaling
"""from sklearn.preprocessing import StandardScaler
sc_X = StandardScaler()
X_train = sc_X.fit_transform(X_train)
X_test = sc_X.transform(X_test)
sc_y = StandardScaler()
y_train = sc_y.fit_transform(y_train)"""

# Fitting Decision Tree Regression to the dataset
from sklearn.tree import DecisionTreeRegressor
regressor = DecisionTreeRegressor(random_state = 0)
regressor.fit(X,y)

# Predicting the new result
# Here y_pred is not going to be the vector of predictions but the predicted salary of 6.5 level
# y_pred = regressor.predict(6.5)

# Visualizing the Regression Results (For higher resolution and smoother curve)
X_grid = np.arange(min(X), max(X), 0.1)
X_grid = X_grid.reshape((len(X_grid), 1))
plt.scatter(X, y, color = 'red')
plt.plot(X_grid, regressor.predict(X_grid), color = 'blue')
plt.title('Truth or Bluff (Regression Model)')
plt.xlabel('Level of Position ()')
plt.ylabel('Salaries')
plt.show()
```

Output:
<img src="{{ site.url }}{{ site.baseurl }}/images/decision_tree/dt2.PNG" alt="linearly separable data">

R code block:
```r
# Importing the dataset
dataset = read.csv('Position_Salaries.csv')
dataset = dataset[2:3]

# Splitting the dataset into the Training set and Test set
# install.packages('caTools')
# library(caTools)
# set.seed(123)
# split = sample.split(dataset$DependentVariable, SplitRatio = 0.8)
# training_set = subset(dataset, split == TRUE)
# test_set = subset(dataset, split == FALSE)

# Feature Scaling
# training_set = scale(training_set)
# test_set = scale(test_set)

# Fitting the Decision Tree Regression Model to the dataset
# Adding a parameter that will set a condition on the split
install.packages('rpart')
library(rpart)
regressor = rpart(formula = Salary ~ ., data = dataset, control = rpart.control(minsplit = 1))

# Predicting a new Result
y_pred = predict(regressor, data.frame(Level = 6.5))

# Visualizing the Decision Tree Regression Model Results (for higher resolution and smoother curve)
library(ggplot2)
x_grid = seq(min(dataset$Level), max(dataset$Level), 0.01)
ggplot() + geom_point(aes(x = dataset$Level, y = dataset$Salary), colour = 'red') +
  geom_line(aes(x = x_grid, y = predict(regressor, newdata = data.frame(Level = x_grid))), colour = 'blue') +
  ggtitle('Truth or Bluff (Decision Tree Regression Model)') +
  xlab('Level') +
  ylab('Salary')
```

Output:
<img src="{{ site.url }}{{ site.baseurl }}/images/decision_tree/dt3.JPG" alt="linearly separable data">

## Applications of Decision Tree Regression
Decision trees have a natural “if … then … else …” construction that makes it fit easily into a programmatic structure. They also are well suited to categorization problems where attributes or features are systematically checked to determine a final category. For example, a decision tree could be used effectively to determine the species of an animal.
