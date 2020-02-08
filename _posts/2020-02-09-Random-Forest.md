---
title: "Machine Learning Project: Random Forest Regression"
date: 2020-02-08
tags: [Machine learning, data science, Random Forest]
header:
    image: "/images/random_forest/rf1.jpg"
excerpt: "Machine Learning, Regression, Data Science"
---

# Random Forest Regression:
A Random Forest is an ensemble technique capable of performing both regression and classification tasks with the use of multiple decision trees and a technique called Bootstrap Aggregation, commonly known as bagging. The basic idea behind this is to combine multiple decision trees in determining the final output rather than relying on individual decision trees.

Approach :
* Pick at random K data points from the training set.
* Build the decision tree associated with those K data points.
* Choose the number Ntree of trees you want to build and repeat step 1 & 2.
* For a new data point, make each one of your Ntree trees predict the value of Y for the data point, and assign the new data point the average across all of the predicted Y values.

---
image: "/images/random_forest/rf2.jpeg"
---

Link to my GitHub page [Random_Forest_Regression](https://github.com/srsapireddy/Machine-Learning-Files-in-Python-and-R/tree/master/Regression/7.%20Random%20Forest%20Regression)
