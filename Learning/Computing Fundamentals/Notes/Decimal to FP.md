---
date_created: 2024-10-03
date_modified: 2024-10-03
document_type: course-note
tags: course course-note
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Notes/Decimal to FP|Decimal to FP]]**
# Decimal to FP
**Overview**
Description:: How to convert from decimal to floating point.

## Note

When converting decimal to [[Floating point numbers|floating point]], it **does not** use 2's compliment. Instead, there is an **offset** or **bias**.

1. Convert to decimal to fixed point
2. Count the number of places needed to move the binary point to the first "10"
3. Insert the sign bit: 1 = negative, 0 = positive
4. Add the offset to the exponent
5. Combine all the parts together: sign, exponent, significand

---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Notes/Decimal to FP|Decimal to FP]]**