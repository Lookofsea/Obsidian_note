---
tags:
  - english
  - MOC
---
```dataview
Table  (date(today) - file.cday)  as "time"
FROM #english or #english/englishpod 
WHERE (date(today) - file.cday) < dur(3 d)
Sort file.ctime desc
```


## [[English pod]]

## [[Daily English Dictation]]

## [[英语残酷共学]]

