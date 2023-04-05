---
quickshare-date: "N/A"
quickshare-url: "Removed"
---
<< [[<% moment(tp.file.title,'YYYY-MM-DD').add(-1,'days').format("YYYY-MM-DD") %>|Yesterday]] | [[<% moment(tp.file.title,'YYYY-MM-DD').format("YYYY") %>-W<% moment(tp.file.title, "YYYY-MM-DD").add(-1,'days').week() %>|This week]] | [[<% moment(tp.file.title,'YYYY-MM-DD').add(1,'days').format("YYYY-MM-DD") %>|Tomorrow]] >> 
> [!DANGER] Today's Focus

# Log

# Process this
```dataview
LIST 
FROM ""
WHERE process = false
LIMIT 5
```
## Tasks 📌
```tasks 
scheduled on <% tp.date.now("YYYY-MM-DD")%>
```
## Today's Notes
### Created
```dataview
LIST
FROM !"Calendar"
WHERE file.cday = date(<%tp.file.title%>)
sort file.ctime.desc
```
### Modified
```dataview
LIST
FROM !"Calendar"
WHERE file.mday = date(<%tp.file.title%>)
sort file.ctime.desc
```
___