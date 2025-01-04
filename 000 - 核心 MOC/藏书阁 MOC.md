---
cssclasses:
  - cards,cards-cols-5,iframe-wide,cards-cover,cards-align-bottom
---


```dataview
table without id ("![]("+ cover +")") as cover, file.link as Title,
readingTime, readingStatus, author as Author, dateformat(readingDate,"yyyy-MM-dd")
from "100 - 🗄 Projects·项目"
where cover != null and readingStatus = "在读" and readingDate.year = 2025
```

```dataview
table without id ("![]("+ cover +")") as cover, file.link as Title,
readingTime, readingStatus, author as Author, dateformat(readingDate,"yyyy-MM-dd")
from "100 - Projects·项目"
where cover != null and readingStatus = "读完" and readingDate.year < 2024
sort readingDate DESC

```




```dataview
TABLE without id
    file.link as "书名",
	author as "作者",
    file.etags AS "标签"
FROM "100 - 🗄 Projects·项目" and #book
```