---
tag: [atlas/scope]
---
# Make time
```dataview 
Table without ID link(file.path, dateformat(file.day, "cccc")) AS Day
from "Calendar/Reviews/Daily" 
Where dateformat(file.day, "kkkk-'W'WW") = dateformat(date(today),"kkkk-'W'WW")
SORT file.day asc
```