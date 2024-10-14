---
date_created: 2024-10-14
date_modified: 2024-10-14
document_type: lecture
tags: course lecture
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/AI Fundamentals/Home|AI Fundamentals]] / **[[Learning/AI Fundamentals/Lectures/03 - Classification|03 - Classification]]**
# 03 - Classification
**Overview**
Description:: Predicting labels, rather than values, and other regression models.
Link:: 

## Section 1

- To predict the correct label (class), instead of the value
- Type: Binary and Multi-Class Classification

Binary: only 2 mutually exclusive categories
Multi-class: more than 2 mutually exclusive categories

Deployment goal is to make the model generalised so it works on most data.

## Logistic Regression

- Used for classification

Assumes a sigmoid function that outputs a number from 0 to 1.
$$
\text{sig}(t) = \frac{1}{1 + e^{-t}}
$$ 
1. Apply linear regression, $f_\theta(x)$
2. Apply sigmoid function from the result of step 1, $\text{sig}(f_\theta(x)$)

Returns the probability of it fitting into one category. Repeated for each class and select highest probability.

## Decision Trees

Keep of splitting from the root until the "leaf" (the categories) is found. Each split results in a rule / if condition to go either left or right.

Each internal node is an *attribute*.

## Random Forest

- Set of decision trees
- Random sampling in data -> random sampling in features to select from
- Attempt to reduce bias
- Select the most favourable decision for the category via voting

*information gain* is used to select which feature to start off with and select the highest.

## k Nearest Neighbour

Find the categories of neighbours and select the most common.

$k$ = distance
If $k$ is too small = sensitive to noise
If $k$ too large = include points from other classes
Choose an odd number for $k$ to eliminate ties

## Support Vector Machine
aka large margin classifier

1. Find a decision boundary that is equidistant to each category (highest margin)

## Confusion matrix

Compare actual and predicted class: true positive, false negative, false positive, true negative.

Accuracy = % of correct classifications = (TP + TN) / All
Error rate = 1 - accuracy or (FP + FN) / All

Precision = % of positive that are actual positive, only looks at positive = TP / (TP + FP)
Recall = true positive rate, includes all data = TP / (TP + FN)
F-measure = mean of precision and recall = 2P * R / (P + R)



---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/AI Fundamentals/Home|AI Fundamentals]] / **[[Learning/AI Fundamentals/Lectures/03 - Classification|03 - Classification]]**

