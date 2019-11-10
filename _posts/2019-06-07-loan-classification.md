---
layout: post
title: "Will the debtor default?"
subtitle: "Predicting loan repayment with classification algorithms including logistic regression, support-vector machine, and decision tree"
nottableau: 'true'
---

In this project, we will use different classification algorithms such as logistic regression, SVM, decision trees, and k-NN to predict whether a certain loan is paid off on time. We will then evaluate and compare their performance to select the best performing algorithm.

You can look at the **[Jupyter notebook](https://nbviewer.jupyter.org/github/h2kh/loan-classification/blob/master/Loan%20classification.ipynb)** here. In this project, I used the following Python libraries: Pandas, Matplotlib, Seaborn,and Scikit-learn. This project, in particular, required a significant amount of feature engineering.

The data includes details of 346 customers whose loan are already paid off or defaulted. Here is what it looks like:

{:refdef: style="text-align: center;"}
![Dashboard snapshot]({{ site.baseimg }}/assets/Capture20.JPG)
{: refdef}

260 people have paid off the loan on time while 86 have gone into collection. In order to understand the breakdown of the data better, we can plot a couple of histograms.

{:refdef: style="text-align: center;"}
![Dashboard snapshot]({{ site.baseimg }}/assets/Capture21.png)
{: refdef}

{:refdef: style="text-align: center;"}
![Dashboard snapshot]({{ site.baseimg }}/assets/Capture22.png)
{: refdef}

{:refdef: style="text-align: center;"}
![Dashboard snapshot]({{ site.baseimg }}/assets/Capture23.png)
{: refdef}

We see that people who get the loan at the end of the week are more likely to default on the loan, so we can create a binary feature 'weekend' that tells us whether the loan began on a weekday or the weekend. Since gender is a binary categorical variable, we can simply code males as 0 and females as 1. As education has more than two levels, we can use one-hot encoding to create indicator variables for each feature. 


Here, you can see the results of the project. We can see that SVM has performed better than all of the other models. One reason for k-NN's relatively poor performance could be the fact that we used uniform weights for all of the neighbors. We could tinker with parameters like these to improve the model. 

{:refdef: style="text-align: center;"}
![Dashboard snapshot]({{ site.baseimg }}/assets/result.JPG)
{: refdef}

If we want somewhat of a balance between model complexity and model performance, decision trees could be a good option (Note: the decision tree below is based on normalized data).


![Decision tree](/assets/dectree.png){:height="650px" width="900px"}

