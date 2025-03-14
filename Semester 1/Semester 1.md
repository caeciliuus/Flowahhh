---
tags:
  - index
  - S1
Type: Index
Date: 2024-12-27
---
```dataview
TABLE date, Type
from #S1   
SORT file.ctime DESC
```

```dataviewjs
const pdfFiles = app.vault.getFiles().filter(file => file.extension === 'pdf' && file.path.includes('S1'))
dv.list(pdfFiles.map(file => dv.fileLink(file.path)))
```