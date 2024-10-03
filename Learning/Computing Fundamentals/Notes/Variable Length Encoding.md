---
date_created: 2024-10-03
date_modified: 2024-10-03
document_type: course-note
tags: course course-note
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Notes/Variable Length Encoding|Variable Length Encoding]]**
# Variable Length Encoding
**Overview**
Description:: 

## Note

Formats like [[UTF-8]] use variable length encoding (VLE) to conserve memory by allocating only the necessary bytes.

If storing one byte, the sequence will start with a singular `0`.
If storing two bytes, the sequence will start with `110` and insert a `10` every 5 bits.
If storing three bytes, the sequence 

---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Notes/Variable Length Encoding|Variable Length Encoding]]**