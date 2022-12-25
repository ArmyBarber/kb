

<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

extra_javascript:
extra:

`$= dv.el("b", "This is some bold text");`

`$= dv.el("b", "This is some text", { cls: "dataview dataview-class", attr: { alt: "Nice!" } });
`

`$= dv.paragraph("This is some text");
`

Basic Field:: Value
**Bold Field**:: Nice!

I would rate this a [rating:: 9]! It was [mood:: acceptable].

`$= dv.current().file.mtime`

```dataviewjs
dv.paragraph(
  dv.pages('"Amazon_clippings"').file.link.slice("", 5).join())
```

Eval
```dataviewjs
dv.evaluate("2 + 2")
```

`$= dv.tryEvaluate("2 + 2")`

Try this
```dataviewjs
dv.paragraph(dv.pages('"Quotes"').file.link.slice("", 5).join())
```

Next
```dataview
TABLE file.name AS "File", rating AS "Rating" FROM "" Limit 10
```
New

```dataview
LIST FROM "" LIMIT 5
```

```dataview
LIST "File Path: " + file.path FROM "" LIMIT 5
```

```dataview
LIST file.path FROM "Amazon_clippings" LIMIT 5
```

```dataview
LIST WITHOUT ID file.path FROM "/" LIMIT 5
```

```dataview
LIST WITHOUT ID file.path FROM "Quotes" LIMIT 5
```

```dataview
TABLE file.day, file.mtime FROM "" LIMIT 5
```

```dataview
LIST "File Path: " + file.path FROM "" LIMIT 5
```

```dataview
TABLE file.day, file.mtime FROM !"Amazon_clippings" LIMIT 5
```

```dataview
TABLE   FROM "Amazon_clippings" LIMIT 5
```

```dataviewjs
dv.pages("#Stalin")
```

