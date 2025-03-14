---
tags:
  - etc
  - index
Type: Index
Date: 2024-07-31
---
```dataview
TABLE date, Type
from #etc   
SORT file.ctime DESC
```
```dataviewjs
const pdfFiles = app.vault.getFiles().filter(file => file.extension === 'pdf' && file.path.includes('Etc'))
dv.list(pdfFiles.map(file => dv.fileLink(file.path)))
```
