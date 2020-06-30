# RegExr was created by gskinner.com, and is proudly hosted by Media Temple.

# Regex Tutorial
## Basic topics
```
Anchors — ^ and $
^The        matches any string that starts with The -> Try it!
end$        matches a string that ends with end
^The end$   exact string match (starts and ends with The end)
roar        matches any string that has the text roar in it
```
```
Quantifiers — * + ? and {}
abc*        matches a string that has ab followed by zero or more c 
abc+        matches a string that has ab followed by one or more c
abc?        matches a string that has ab followed by zero or one c
abc{2}      matches a string that has ab followed by 2 c
abc{2,}     matches a string that has ab followed by 2 or more c
abc{2,5}    matches a string that has ab followed by 2 up to 5 c
a(bc)*      matches a string that has a followed by zero or more copies of the sequence bc
a(bc){2,5}  matches a string that has a followed by 2 up to 5 copies of the sequence bc
```
```
OR operator — | or []
a(b|c)     matches a string that has a followed by b or c (and captures b or c) -> Try it!
a[bc]      same as previous, but without capturing b or c
Character classes — \d \w \s and .
\d         matches a single character that is a digit -> Try it!
\w         matches a word character (alphanumeric character plus underscore) -> Try it!
\s         matches a whitespace character (includes tabs and line breaks)
.          matches any character -> Try it!
```


# CSS Grid Reference
CSS Grid Layout is the most powerful layout system available in CSS. It is a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a 1-dimensional system

```
display
Defines the element as a grid container and establishes a new grid formatting context for its contents.

Values:

grid – generates a block-level grid
inline-grid – generates an inline-level grid
```


* grid-template-columns
* grid-template-rows
```
.container {
  grid-template-columns:  ... |   ...;
  grid-template-rows:  ... |   ...;
}
```



# Responsive design with CSS Grid

In the same way that flexbox gave us a way to layout block elements next to each other, CSS grid lets us not only arrange elements in a row or a column, but in multiple rows and columns. Finally two dimensional layouts are becoming **simpler**!


