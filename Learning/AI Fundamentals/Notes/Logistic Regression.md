---
date_created: 2024-10-14
date_modified: 2024-10-14
document_type: course-note
tags: course course-note
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/AI Fundamentals/Home|AI Fundamentals]] / **[[Learning/AI Fundamentals/Notes/Logistic Regression|Logistic Regression]]**
# Logistic Regression
**Overview**
Description:: Linear classification model using linear regression and a sigmoid.

## Note

Logistic regression is a type of [[Regression model|regression model]] that predicts categories and is used during [[Classification|classification]]. The [[Regressor|regressor]] is a combination of a [[Linear Regression Model|linear regression model]] and a [[Sigmoid function|sigmoid function]] to give a probability that $x$ fits into the provided class.

1. Apply linear regression, $f_\theta(x)$
2. Apply sigmoid function from the result of step 1, $\text{sig}(f_\theta(x)$)

The output is a number from 0 to 1 which represents the probability that it fits into the class. Repeat this process for each category and select the category with the highest probability.

---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/AI Fundamentals/Home|AI Fundamentals]] / **[[Learning/AI Fundamentals/Notes/Logistic Regression|Logistic Regression]]**