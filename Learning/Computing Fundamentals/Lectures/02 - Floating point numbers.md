---
date_created: 2024-10-02
date_modified: 2024-10-02
document_type: lecture
tags: course lecture
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Lectures/02 - Floating point numbers|02 - Floating point numbers]]**
# 02 - Floating point numbers
**Overview**
Description:: 
Link:: 

## Fixed point

- Limited precision
- Small maximum size

## Standard form notation

In the form: `a * b^c` where
- a = significand
- b = base
- c = exponent

Allows compact and efficient way to represent small **and** large numbers.
- as long as they're not very precise...

Increase exponent = bigger number but less precise
Increase significand = smaller number but more precise

Therefore, can't be large and small at the same time.
- To get around this, store the "large" and "small" numbers separately 

## Single precision

- 23 bit significand
- 8 bit exponent
- 127 offset (for negative numbers, instead of 2s compliment)

## Double precision

- 52 bit significand
- 11 bit exponent
- 1023 offset


---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Lectures/02 - Floating point numbers|02 - Floating point numbers]]**

