---
date_created: 2024-10-14
date_modified: 2024-10-14
document_type: lecture
tags: course lecture
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/AI Fundamentals/Home|AI Fundamentals]] / **[[Learning/AI Fundamentals/Lectures/03 - Classification|03 - Classification]]**
# 03 - Classification
**Overview**
Description:: 
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

*informaton gain* is used to select which feature to start off with (hig)

---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/AI Fundamentals/Home|AI Fundamentals]] / **[[Learning/AI Fundamentals/Lectures/03 - Classification|03 - Classification]]**

