## Google Search Operators

| Search Operator | Description |
| --- | --- |
| " " | Search for results that mention a word or phrase |
| OR  | Search for results related to X or Y |
| \|  | Same as OR |
| AND | Search for results related to X and Y |
| \-  | Search for results that don't mention a word or phrase |
| \*  | Wildcard matching any word or phrase |
| ( ) | Group multiple searches |
| define: | Search for definition of a word or phrase |
| cache: | Find the most recent cache of a website |
| filetype: | Search for particulat type of file |
| ext: | Same as filetype |
| site: | Search for results from a particular website |
| related: | Search for sites related to a given domain |
| intitle: | Search for pages with a particular word in the title tag |
| allintitle: | Search for pages with multiple words in the title tag |
| inurl: | Search for pages with a particular word in the URL |
| allinurl: | Search for pages with multiple words in the URL |
| intext: | Search for pages with particular word in their content |
| allintext: | Search for pages with multiple word in their content |
| weather: | Search for weather in a location |
| stocks: | Search for stock information for a ticker |
| map: | Force Google to show map results |
| movie: | Search for information about a movie |
| in:  | Convert one unit to another |
| source: | Search for results from a particular source in Google News |
| before: | Search for results from before a particular date |
| after: | Search for results from after a particular date |
| 94fbr (file) | Code for direct download a file or binary, like .sscexe

&nbsp;

## Google Search Examples

```bash
# Search for entire phrase
"Javascript arrays"

# Search for entire phrase but only on www.w3schools.com
site:www.w3schools.com "javascript arrays"

# Search for a phrase but without word "build"
"javascript developer" -build

# Search for PDF file with phrase javascript
filetype:pdf "javascript"

# Search for one phrase OR another
"javascript dupa" OR "haskell dupa"

# Search for one phrase AND another
"javascript dupa" AND "haskell dupa"

# Search for a phrase with wildcard * (any string between two strings)
"unexpected * after top level declaration"

# Search for a wildcard phrase but withour word "JetBrains" but with another phrase "Ran go test"
"unexpected * after top level declaration" -JetBrains AND "Ran go test"

# Search for PDF file with string AND another string 
"OUT OF THE BODY" AND "CIA" filetype:pdf

# Search for string in URL (address) on a particular site
inurl:shared site:rawtherapee.com

```