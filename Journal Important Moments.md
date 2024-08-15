---
tags: meta
---
_About our moments together, especially of appreciation, joy, challenge. Also:_

- Learn through my [[Decision Journal]]
- Thoughts in progress are in [[Revisit Incomplete Thoughts]]

# 🌱 Moments I've written down:
---
```dataview
CALENDAR file.ctime
```
---

> [!Multi-column]
>
> > [!cite]+ Moments Together
> > ### 🎵 🏕️
> >
> > ```dataview
> > TABLE WITHOUT ID link(file.path, regexreplace(file.name, "^\d{4}-\d{2}-\d{2}( - )?", "")) AS Moments,
> > dateformat(file.ctime, "DD") as "Created"
> > FROM #moment
> > WHERE !contains(file.path, "Template")
> > sort file.ctime desc
> > ```
>
> > [!cite]+ Other Reflections
> > 
> >### 💭
> >
> > ```dataview
> > TABLE WITHOUT ID link(file.path, regexreplace(file.name, "^\d{4}-\d{2}-\d{2}( - )?", "")) AS Moments,
> > dateformat(file.ctime, "DD") as "Created"
> > FROM #reflection
> > WHERE !contains(file.path, "Template")
> > sort file.ctime desc
> > ```

## Past Moments
```dataview
TABLE WITHOUT ID link(file.path, regexreplace(file.name, "^\d{4}-\d{2}-\d{2}( - )?", "")) AS "",
dateformat(file.ctime, "DD") as "Created"
WHERE !contains(file.path, "Template") AND !contains(file.tags, "meta")
SORT file.ctime desc
```
