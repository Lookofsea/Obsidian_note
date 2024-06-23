---
tags:
  - english
  - MOC
---
```dataview
Table  (date(today) - file.cday)  as "time"
FROM #english
WHERE (date(today) - file.cday) < dur(3 d)
Sort file.ctime desc
```
## 英语口语听力阅读学习

[[English pod]]

[[Daily English Dictation]]

[[英语残酷共学]]

