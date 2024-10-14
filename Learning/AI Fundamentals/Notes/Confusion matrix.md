---
date_created: 2024-10-14
date_modified: 2024-10-14
document_type: course-note
tags: course course-note
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/AI Fundamentals/Home|AI Fundamentals]] / **[[Learning/AI Fundamentals/Notes/Confusion matrix|Confusion matrix]]**
# Confusion matrix
**Overview**
Description:: Used for evaluating classification models.

## Note

A confusion matrix can be used to evaluate a [[Classification|classification]] model. It compares what the actual class against the predicted class.

| Actual/Predicted | True                | False               |
| ---------------- | ------------------- | ------------------- |
| True             | True Positive (TP)  | False Negative (FN) |
| False            | False Positive (FP) | True Negative (TN)  |

The accuracy, the percentage of correct classifications, can be calculated using $\frac{\text{TP} + \text{TN}}{\text{All}}$. From that, the error rate can be calculated by doing $1 - \text{accuracy}$ or $\frac{\text{FP} + \text{FN}}{\text{All}}$.

The precision, the percentage of positives that are actually positive (only looking at positive data) = $\frac{\text{TP}}{\text{TP} + \text{FP}}$.

The recall, the true positive rate which includes all data = $\frac{\text{TP}}{\text{TP} + \text{FN}}$.

The F-measure is the mean of precision and recall. It can be calculated by doing:
$$
\frac{2}{\frac{1}{P} + \frac{1}{R}} = 2 \times \frac{PR}{P + R}
$$



---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/AI Fundamentals/Home|AI Fundamentals]] / **[[Learning/AI Fundamentals/Notes/Confusion matrix|Confusion matrix]]**