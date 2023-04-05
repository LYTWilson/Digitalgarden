---
tag: [module, atlas/scope]
year: 
semester: 
credit:  
grade: 
---
up:: [[College courses]]
lecturer::
textbook:: 
___
# Outline

# Lectures
```dataview
LIST
FROM #lecture AND [[<%tp.file.title%>]] 
```
# Projects
```dataview
TABLE WITHOUT ID 
file.link as "Project", deadline AS "Deadline"
FROM #project
WHERE module = [[<%tp.file.title%>]]
SORT deadline asc
```
# Classmates
