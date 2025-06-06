---
title: Dashboard
category: MOC
type: Dashboard
tags:
  - MOC
  - Dashboard
  - Index
date: 2025-02-20
---
# School Notes
- [[A Levels MOC]]
	- [[Computer Science MOC]]
	- [[Music MOC]]
	- [[Maths MOC]]
	- [[Economics MOC]]
# Personal Learning

# Personal Life
- [[Daily Note MOC]]
- [[Archive MOC]]
- [[Clippings MOC]]
# Projects
- [[Projects MOC]]
# Recent Notes
```dataview
TABLE type, date
WHERE date >= date(today) - dur(7 days)
AND !contains(file.path, "09. Templates")
SORT date DESC
```
