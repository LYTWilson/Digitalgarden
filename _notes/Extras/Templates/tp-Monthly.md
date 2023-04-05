[[<% moment(tp.file.title, "YYYY-MMM").add(-1, 'months').format("YYYY-MMM") %>]] | [[<% moment(tp.file.title,'YYYY-MMM').format('YYYY') %>]] | [[<% moment(tp.file.title, "YYYY-MMM").add(+1, 'months').format("YYYY-MMM") %>]] 
# This month

## Reflection
```dataview
TABLE 
	log-reflection as Reflection
FROM "Calendar/Reviews/Daily"
WHERE log-reflection
```


