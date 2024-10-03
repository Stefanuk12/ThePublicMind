---
date_created: 2024-10-03
date_modified: 2024-10-03
document_type: course-note
tags: course course-note
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Notes/Floating point numbers|Floating point numbers]]**
# Floating point numbers
**Overview**
Description:: 

## Note

Floating point numbers allow computers to store fractions and much larger (or smaller) numbers.

### Single precision

- 23 bit significand
- 8 bit exponent
- 127 offset

### Double precision

- 52 bit significand
- 11 bit exponent
- 1023 offset

### Calculation

1. Convert to decimal to fixed point
2. Count the number of places needed to move the binary point to the first "10"
3. Insert the sign bit: 1 = negative, 0 = positive
4. Add the offset to the exponent
5. Combine all the parts together: sign, exponent, significand

### Warnings
 - Floats are never equal, e.g. `0.1 + 0.1 + 0.1 != 0.3`
 - Repeated calculations = more inaccurate
 - Don't use to count...

---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Notes/Floating point numbers|Floating point numbers]]**