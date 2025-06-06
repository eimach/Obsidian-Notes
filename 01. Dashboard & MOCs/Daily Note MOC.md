Links: [[Dashboard]]
## Incomplete Tasks
``` dataview
task from "00. Daily"
where !completed and !contains(text, "Taken Inhaler") and !contains(text, "x")
sort file.mtime desc
limit 15
```
## Last 5 Days
``` dataview
list from "00. Daily"
sort file.ctime desc
limit 5
```
## All Daily Notes
``` dataview
list from "00. Daily"
sort file.name desc
```