---
tags: meta
---
Some thoughts don't start out as complete but can grow with time 🍃


```dataview
TABLE WITHOUT ID 
link(file.path, regexreplace(file.name, "^\d{4}-\d{2}-\d{2}( .{3} – )?", "")) as Moments, Mood, dateformat(file.ctime, "DD") as "Created"
FROM #revisit
WHERE !contains(file.path, "Template")
SORT created desc
```
