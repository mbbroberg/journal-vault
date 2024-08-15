---
tags: meta
---

> [!anchor]+
> Go down to a local drugstore and buy a very cheap notebook and start keeping track of your decisions. And the specific idea is whenever you’re making a consequential decision, something going in or out of the portfolio, just take a moment to think, ==write down what you expect to happen, why you expect it to happen== and then [...] ==how you feel about the situation, both physically and even emotionally==. Just, how do you feel? I feel tired. I feel good, or this stock is really draining me. Whatever you think.
> ~ _[[Daniel Kahneman]]_


```dataview
TABLE WITHOUT ID 
link(file.path, regexreplace(file.name, "^\d{4}-\d{2}-\d{2}( .{3} – )?", "")) as Moments, Mood, dateformat(file.ctime, "DD") as "Created"
FROM #decision
SORT created desc
```
