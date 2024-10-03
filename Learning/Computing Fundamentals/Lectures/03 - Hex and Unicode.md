---
date_created: 2024-10-03
date_modified: 2024-10-03
document_type: lecture
tags: course lecture
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Lectures/03 - Hex and Unicode|03 - Hex and Unicode]]**
# 03 - Hex and Unicode
**Overview**
Description:: 
Link:: 

## Hexadecimal

Base-16
- Easier to read, interpret and remember than binary
- Can be easily converted to binary and back
	- 1 byte = 2 hex digits

0-9 then A-F (to represent 10 to 15)

`h` in ASM on datum = hex

## ASCII

Many versions, we now use 1987 ver. Previous versions didn't have lowercase, `_`, etc.

- 7 bit, not 8 because old

## Unicode

- Successor to ASCII
- 21 bits, as many more aren't needed and allows storage optimisations
- U+`num` = Unicode character
- Doesn't control styling

### UTF-8
- variable length (VLA) from 1-4 bytes
- ASCII = valid Unicode $\therefore$ extended ASCII is not

### Planes

- Plane 1
	- 0000-FFFF
	- Basic multilingual
	- Latin, Greek, Maths, Chinese, ...
- Plane 1 = 10000-1FFFF
	- Supplementary multilingual
- Plane 2 = 20000-2FFFF
	- Supplementary ideographic plane
- Plane 3-13 = 30000-DFFFF
	- Reserved for expansion
- Plane 14 = E0000-EFFFF
	- Supplementary special purpose plane
- Plane 15-16 = F0000-10FFFF
	- Private use areas

---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Lectures/03 - Hex and Unicode|03 - Hex and Unicode]]**

