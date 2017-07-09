
``` yaml
The design goals for YAML:

- YAML is easily readable by humans.
- YAML data is portable between programming languages.
- YAML matches the native data structures of agile languages.
- YAML has a consistent model to support generic tools.
- YAML supports one-pass processing.
- YAML is expressive and extensible.
- YAML is easy to implement and use.
```

# Awesome YAML (Ain't Markup Language)

A collection of Awesome YAML (Ain't Markup Language) goodies for structured (meta) data in text.


#### _Contributions welcome. Anything missing? Send in a pull request. Thanks._


## Formats

### "Standard" YAML

**YAML HQ**

- [`yaml.org`](http://www.yaml.org) - official YAML website by Clark C. Evans
  - [YAML Spec v1.2](http://yaml.org/spec/1.2/spec.html) - 3rd edition, Oct 2009 
  - [YAML Quick Reference Card](http://www.yaml.org/refcard.html) - one-page cheat sheet

### "Safe" YAML



## Articles

- [**YAML Quick Reference (Cheat Sheet) for Jekyll Data Files, Front Matter and Collections**](https://github.com/planetjekyll/quickrefs/blob/master/YAML.md), Planet Jekyll
- [**Learn YAML in Y Minutes**](https://learnxinyminutes.com/docs/yaml), Learn X in Y minutes series, 
- [**Deep dive into TOML, JSON and YAML**](https://gohugohq.com/howto/toml-json-yaml-comparison/),  Go Hugo HQ, Dec 2016
- [**YAML @ Wikipedia**](https://en.wikipedia.org/wiki/YAML)


## Tips & Gotchas


**Strings with Colons (`:`)**

When to use quotes for your strings?

If your string includes a colon (`:`) followed by a space you MUST quote your string. Otherwise, the colon is interpreted as a key/value separator (e.g. _key: value_). Example:

``` yaml
title: "Text Processing with Ruby: Extract Value from the Data That Surrounds You"
title: "Sinatra: Up and Running - Ruby for the Web, Simply"
title: "Using JRuby: Bringing Ruby to Java"
```

Note: You can quote your strings using double quotes (`""`) e.g. "Using JRuby: Bringing Ruby to Java" 
or single quotes(`''`) e.g. 'Using JRuby: Bringing Ruby to Java'.



**No Tabs (\t) for Indentation - Use Spaces, Period**

Note: Always use spaces for indentation, period. 
Make sure no tabs (`\t`) have somehow ended up in your datafile leading to
unexpected results.



**Predefined Boolean 'n' No Value Constants - True/False, Yes/No, On/Off, ~/Null**

Note: The boolean `true` and `false` constants e.g.:

```
true, True, TRUE
y, Y, yes, YES, YES
on, ON, ON
false, False, FALSE
n, N, no, No, NO
off, Off, OFF
```

will become boolean values e.g. `true` or `false`.  If you want end-up with a string e.g.:

``` yaml
recommend: Yes       # note: will become => true (boolean)
```

make sure you use a quoted version e.g.:

``` yaml
recommend: "Yes"     # note: will become => "Yes" (string)
```


Note: The same holds for the no value null constants e.g.:

``` yaml
~
null, Null, NULL
```

will become => `null` (no value). Note: A key without a value will end-up with a `null` value (and not an empty string, for example). To get an empty string use `""` e.g.:

``` yaml
key1:           # note: value will become => null (no value); same as key1: null  or key1: ~
key2: ""        # note: value will become => "" (string)
```



## JSON 

_JSON is (a subset of) YAML, that is YAML is JSON but JSON is NOT YAML ;-)_

Example: Use the inline style for lists (that is, JSON arrays)
and hashes (that is, JSON objects) for an alternative "JSON-style" syntax:


``` json
[
  { "title": "football.db - Open Football Data",
    "url":   "https://github.com/openfootball" 
  },
  { "title": "beer.db - Open Beer, Brewery 'n' Brewpub Data",
    "url":   "https://github.com/openbeer" 
  }
]
```

is the same as:

``` yaml
- title : football.db - Open Football Data
  url   : https://github.com/openfootball
- title : beer.db - Open Beer, Brewery 'n' Brewpub Data
  url   : https://github.com/openbeer
```




## Tools & Services

- [**YAML Linter @ yamllint.com**](http://www.yamllint.com) - online YAML validator / checker
- [**YAML Validator @ Code Beautify**](https://codebeautify.org/yaml-validator) - online YAML validator / checker



## Misc

- [**Feed.TXT**](https://feedtxt.github.io) - web feed format with meta data in YAML
- [**YAML @ Stackoverflow**](https://stackoverflow.com/tags/yaml/info) - frequently asked questions (and answers) about YAML


## Meta

**License**

![](https://publicdomainworks.github.io/buttons/zero88x31.png)

The awesome list is dedicated to the public domain. Use it as you please with no restrictions whatsoever.

**Questions? Comments?**

Post them to the [wwwmake forum](http://groups.google.com/group/wwwmake). Thanks!
