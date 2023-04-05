---
tag: [source/book]
status: 
title: {{title}}
category: {{category}}
publisher: {{publisher}}
publish_date: {{publishDate}}
total_page: {{totalPage}}
isbn: {{isbn10}} {{isbn13}}
cover: {{coverUrl}}
rating: 
---
![cover|150]({{coverUrl}})
author:: <%=book.authors.map(author => `[[${author}]]`).join(', ')%>
# Quotes
