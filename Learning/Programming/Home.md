---
date_created: 2024-09-24
date_modified: 2024-09-24
document_type: course
tags: sub-dashboard course
---
[[Learning/Learning Dashboard|Learning Dashboard]] / **[[Learning/Programming/Home.md|Programming]]**
# Programming
**Overview**
Title:: Programming
Subject:: Computer Science
Description:: N/A
Completed:: false
Link:: <% tp.file.cursor(1) %>


## Actions
```button
name + Add lecture
type note(Learning/Programming/Lectures/unnamed lecture) template
action learning/Course lecture
templater true
class tailwind-button-white
```

```button
name + Add assignment
type note(Learning/Programming/Assignments/unnamed assignment) template
action learning/Course assignment
templater true
class tailwind-button-white
```

```button
name + Add note
type note(Learning/Programming/Notes/unnamed note) template
action learning/Course note
templater true
class tailwind-button-white
```


## Lectures
```dataviewjs
for (let group of dv.pages('"Learning/Programming" and #lecture').groupBy(p => p.lecture)) {
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
for (let group of dv.pages('"Learning/Programming" and #assignment').groupBy(p => p.lecture)) {
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
for (let group of dv.pages('"Learning/Programming" and #course-note').groupBy(p => p.lecture)) {
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
[[Learning/Learning Dashboard|Learning Dashboard]] / **[[Learning/Programming/Home.md|Programming]]**