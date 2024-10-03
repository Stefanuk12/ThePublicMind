---
date_created: 2024-10-03
date_modified: 2024-10-03
document_type: course-note
tags: course course-note
---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Notes/Unicode|Unicode]]**
# Unicode
**Overview**
Description:: Gives each character a numerical value.

## Note

Unicode is the successor to [[ASCII]] and instead of only using 7 bits, it uses **21 bits** which yields around over a million possible characters. It's useless to have more, especially considering that we only currently use around 10%. 21 bits also allows for some storage optimisations.

Unicode gives each character a numerical value, but it does **not** tell the computer how to store the value. However, it does define [[Unicode Planes|planes]] which allocate blocks of the available space to specific purposes.

---
[[Learning/Learning Dashboard|Learning Dashboard]] / [[Learning/Computing Fundamentals/Home|Computing Fundamentals]] / **[[Learning/Computing Fundamentals/Notes/Unicode|Unicode]]**