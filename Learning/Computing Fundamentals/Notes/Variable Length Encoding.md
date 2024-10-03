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
If storing two bytes, the sequence will start with `110` and insert a `10` every 6 bits once.
If storing three bytes, the sequence will start with `1110` and insert `10` every 6 bits twice.
If storing four bytes, the sequence will start with `11110` and insert `10` every 6 bits thrice.

To summarise, it starts by filling one byte with $N$ number of `1`s, except for when $N = 1$, then a `0`. It then fills the remaining of the byte with any data. Each new byte will start with a leading `10`.

When decoding, the leading bits are removed and the remaining bits are concatenated to form the actual value we want.

---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Notes/Variable Length Encoding|Variable Length Encoding]]**