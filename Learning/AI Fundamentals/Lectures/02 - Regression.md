---
date_created: 2024-10-07
date_modified: 2024-10-07
document_type: lecture
tags: course lecture
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/AI Fundamentals/Home|AI Fundamentals]] / **[[Learning/AI Fundamentals/Lectures/02 - Regression|02 - Regression]]**
# 02 - Regression
**Overview**
Description:: 
Link:: 

## Introduction

Regression = an **algorithm** that creates a model to predict a model. It is **not** the model itself.
- Useful when little data is available
- Easy to interpret
- Robust
- Fast

- Input = Independent
- Output = Dependant 

It establishes a relationship between the features (inputs) and label (output).

## Types of regression

- Univariate (1 feature)
	- Linear
	- Non-Linear
- Multivariate (2+ features)
	- Linear
	- Non-Linear

## Splitting the dataset

- Training
	- Apply the algorithm to this split, to establish the relationship
- Validation
	- During training, generate predictions on unseen data and compare to known
	- To access the performance of the model
	- Can be used for model hyper-parameter tuning
- Test

## Pre-processing

- Transformation
	- Convert from text to numerical
- Cleaning
	- Remove duplicates
	- Deal with missing values (predict or remove data)

## Other terminology

- Epoch/iteration = full pass over the training data
	- Do many iterations until the model converges (minimal error, *look at this more*) or a maximum reached
- Algorithm -> predictive model
	- Training an algorithm -> validating the predictive model

## Linear Regression Model

The regressor is $f_0(x) = \theta_0 + \theta_1x$ which is a $y = mx + c$ model.
- Parameters here are $\theta_0$ and $\theta_1$

	To measure the accuracy of the parameters, we use a loss function. In this case, we use the mean square error:
$$
L(\theta_0, \theta_1) = \frac{1}{m}\sum_{i=1}^{m}{(f_\theta(x_i) - y_i)^2}
$$
The parameters are initially random, then the model is repeated with different parameters, trying to minimise $L$. The model stops when the best result is achieved or until the maximum iterations has been reached.

*why do we square?*
- removes negatives
- always $\geq$ 0
*how does the model refine the parameters?*
- updated in opposite direction to gradient
- size of steps taken given by a learning rate
- -> least squares *research this*

Be aware of noise in the data!

Difference between predicted value and label = residual/loss function
- This can be used to measure the accuracy and calculate a MSE as mentioned previously

Since we squared the error, we can sqrt it to get the estimated loss. This means that the incorrect predictions are around off by that RMSE.

$R^2$ , the coefficient of determination, can also be calculated which tells us the correlation between $x$ and $y$.
- It gives a value between 0 and 1
- 1 = model explains all of the variation in the data
- Closer to 1 is better

## Multivariate Linear Regression

The regressor is changed to be:
$$
f_0(x) = \theta + \theta_1x + \theta_2x_2 + \dots
$$

and the loss function is changed to include each parameter.

$$
L(\theta_0, \theta_1, \theta_2, \dots) = \frac{1}{m}\sum_{i=1}^{m}{(f_\theta(x_i) - y_i)^2}
$$

---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/AI Fundamentals/Home|AI Fundamentals]] / **[[Learning/AI Fundamentals/Lectures/02 - Regression|02 - Regression]]**

