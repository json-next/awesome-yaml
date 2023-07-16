
## Article Meta Data (Front Matter) Sample



### TOML (Tom's Obvious, Minimal Language)

Note: Use `+++`to begin and end meta data (front matter) block.


``` toml
+++
date = "2016-12-14T21:27:05.454Z"
publishdate = "2016-12-14T21:27:05.454Z"

title = "Deep dive into TOML, JSON and YAML"
tags = ["toml","yaml","json", "front matter"]

type = "article"

[amp]
    elements = []
    
[article]
    lead = "Lorem ipsum."
    category = "frontmatter"
    related = []

[sitemap]
  changefreq = "monthly"
  priority = 0.5
  filename = "sitemap.xml"
+++
```


### YAML (Ain't Markup Language)

Note: Use `---` to begin and end meta data (front matter) block.

``` yaml
---
date: '2016-12-14T21:27:05.454Z'
publishdate: '2016-12-14T21:27:05.454Z'
title: Deep dive into TOML, JSON and YAML
tags:
- toml
- yaml
- json
- front matter
type: article
amp:
  elements: []
article:
  lead: Lorem ipsum.
  category: frontmatter
  related: []
sitemap:
  changefreq: monthly
  priority: 0.5
  filename: sitemap.xml
---
```

### JSON (JavaScript Object Notation)

Note: Use `{ }` or `[ ]` to begin and end meta data (front matter) block.

``` json
{
    "date" : "2016-12-14T21:27:05.454Z",
    "publishdate" : "2016-12-14T21:27:05.454Z",
    "title" : "Deep dive into TOML, JSON and YAML",
    "tags" : ["toml","yaml","json", "front matter"],
    "type" : "article",
    "amp" : {
        "elements" : []
    },
    "article" : {
        "lead" : "Lorem ipsum.",
        "category" : "frontmatter",
        "related" : []
    },
    "sitemap" : {
      "changefreq" : "monthly",
      "priority" : 0.5,
      "filename" : "sitemap.xml"
    }
}
```

### JSON5 (JavaScript Object Notation)

Note: Use `{ }` or `[ ]` to begin and end meta data (front matter) block.

``` json5
{
    date : "2016-12-14T21:27:05.454Z",
    publishdate : "2016-12-14T21:27:05.454Z",
    title : "Deep dive into TOML, JSON and YAML",
    tags : ["toml","yaml","json", "front matter"],
    type : "article",
    amp : {
        elements : []
    },
    article : {
        lead : "Lorem ipsum.",
        category : "frontmatter",
        related : []
    },
    sitemap : {
      changefreq : "monthly",
      priority : 0.5,
      filename : "sitemap.xml"
    }
}
```

