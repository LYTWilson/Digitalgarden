---
tag: [atlas/scope]
---
# Notes that need to be processed
```dataview
TABLE rows.file.link AS Notes
FROM #lecture and !"Extras"
WHERE process = false
group by up AS Module
```

