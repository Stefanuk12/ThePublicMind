---
date_created: 2024-09-24
date_modified: 2024-10901-24
document_type: course
tags: sub-dashboard course
---
[[Learning/Learning Dashboard|Learning Dashboard]] / **[[Learning/Computational Thinking/Home.md|Computational Thinking]]**
# Computational Thinking
**Overview**
Title:: Computational Thinking
Subject:: Computer Science
Description:: N/A
Completed:: false
Link:: 


## Actions
```button
name + Add lecture
type note(Learning/Computational Thinking/Lectures/unnamed lecture) template
action learning/Course lecture
templater true
class tailwind-button-white
```

```button
name + Add assignment
type note(Learning/Computational Thinking/Assignments/unnamed assignment) template
action learning/Course assignment
templater true
class tailwind-button-white
```

```button
name + Add note
type note(Learning/Computational Thinking/Notes/unnamed note) template
action learning/Course note
templater true
class tailwind-button-white
```


## Lectures
```dataviewjs
for (let group of dv.pages('"Learning/Computational Thinking" and #lecture').groupBy(p => p.lecture)) {
	dv.table(["Lecture", "Description", "Date created"], 
		group.rows 
			.sort(k => k.file.ctime, 'desc')
			.map(k => [
			k.file.link, 
			k['description'],
			k.file.ctime.year+"-"+k.file.ctime.month+"-"+k.file.ctime.day
			]))
}
```


## Assignments

```dataviewjs
for (let group of dv.pages('"Learning/Computational Thinking" and #assignment').groupBy(p => p.lecture)) {
	dv.table(["Lecture", "Completed", "Date created"], 
		group.rows 
			.sort(k => k.file.ctime, 'desc')
			.map(k => [
			k.file.link, 
			k['completed'],
			k.file.ctime.year+"-"+k.file.ctime.month+"-"+k.file.ctime.day
			]))
}
```


## Notes
```dataviewjs
for (let group of dv.pages('"Learning/Computational Thinking" and #course-note').groupBy(p => p.lecture)) {
	dv.table(["Note", "Description"], 
		group.rows 
			.sort(k => k.file.ctime, 'desc')
			.map(k => [
			k.file.link, 
			k['description']
			]))
}
```


---
[[Learning/Learning Dashboard|Learning Dashboard]] / **[[Learning/Computational Thinking/Home.md|Computational Thinking]]**