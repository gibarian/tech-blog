---
title: '- Search'
---

## Google Search Operators

| Search Operator | Description                                                |
|-----------------|------------------------------------------------------------|
| " "             | Search for results that mention a word or phrase           |
| OR              | Search for results related to X or Y                       |
| \|              | Same as OR                                                 |
| AND             | Search for results related to X and Y                      |
| \-              | Search for results that don't mention a word or phrase     |
| \*              | Wildcard matching any word or phrase                       |
| ( )             | Group multiple searches                                    |
| site:           | Search for results from a particular website               |
| filetype:       | Search for particulat type of file                         |
| ext:            | Same as filetype                                           |
| inurl:          | Search for pages with a particular word in the URL         |
| 94fbr:          | Code for direct download a file or binary, like .sscexe    |
|                 |                                                            |
| define:         | Search for definition of a word or phrase                  |
| cache:          | Find the most recent cache of a website                    |
| related:        | Search for sites related to a given domain                 |
| intitle:        | Search for pages with a particular word in the title tag   |
| allintitle:     | Search for pages with multiple words in the title tag      |
| allinurl:       | Search for pages with multiple words in the URL            |
| intext:         | Search for pages with particular word in their content     |
| allintext:      | Search for pages with multiple word in their content       |
| stocks:         | Search for stock information for a ticker                  |
| source:         | Search for results from a particular source in Google News |
| before:         | Search for results from before a particular date           |
| after:          | Search for results from after a particular date            |

&nbsp;

## Google Search Examples

- [google.com](https://google.com)

---

Search for entire phrase
```yaml
"Javascript arrays"
```

Search for entire phrase but only on www.w3schools.com
```yaml
site:www.w3schools.com "javascript arrays"
```

Search for a phrase but without word "build"
```yaml
"javascript developer" -build
```

Search for PDF file with phrase javascript
```yaml
filetype:pdf "javascript"
```

Search for one phrase OR another
```yaml
"javascript foobarbaz" OR "haskell foobarbaz"
```

Search for one phrase AND another
```yaml
"javascript foobarbaz" AND "haskell foobarbaz"
```

Search for a phrase with wildcard * (any string between two strings)
```yaml
"unexpected * after top level declaration"
```

Search for a wildcard phrase but withour word "JetBrains" but with another phrase "Ran go test"
```yaml
"unexpected * after top level declaration" -JetBrains AND "Ran go test"
```

Search for PDF file with string AND another string
```yaml
"OUT OF THE BODY" AND "CIA" filetype:pdf
```

Search for 'shared' string in URL (address) on a particular site
```yaml
inurl:shared site:rawtherapee.com
```

Search for skype installers and linux installer of enemy territory
```yaml
94fbr skype
94fbr etlegacy-v2.83.2-x86_64.sh
```