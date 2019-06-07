---
layout: post
title: "Will the debtor default? Predicting loan repayment with classification algorithms"
---

In this project, we will use different classification algorithms such as logistic regression, SVM, decision trees, and k-NN to predict whether a certain loan is paid off on time. We will then evaluate and compare their performance to select the best performing algorithm.

You can look at the [Jupyter notebook here](https://nbviewer.jupyter.org/github/h2kh/loan-classification/blob/master/Loan%20classification.ipynb). This project, in particular, required a significant amount of feature engineering.

Here, you can see the results of the project. We can see that SVM has performed better than all of the other models. One reason for k-NN's relatively poor performance could be the fact that we used uniform weights for all of the neighbors. We could tinker with that to improve the model. 

![perform](/assets/result.JPG)

If we want somewhat of a balance between model complexity and model performance, decision trees could be a good option.

![tree](/assets/dectree.png)
