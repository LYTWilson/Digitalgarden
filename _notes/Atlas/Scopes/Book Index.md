---
tag: atlas/scope
---
```dataviewjs
for (let group of dv.pages('#source/book and !"Extras/Templates"').groupBy(p => p.status)) {
	dv.header(3, group.key);
	dv.table(["Book", "Author", "Rating"],
	group.rows
		.sort(k => k.rating, 'desc')
		.map(k => [k.file.link, k["author"], k.rating]))
}
```
