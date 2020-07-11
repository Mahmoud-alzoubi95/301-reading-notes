# read 11 : EJS
EJS is a simple templating language that lets you generate HTML markup with plain JavaScript

* It integrates with the Express View Engine.

We must indtall it before working :
`npm install ejs`
 To use it :
 ```
 let ejs = require('ejs');
let people = ['geddy', 'neil', 'alex'];
let html = ejs.render('<%= people.join(", "); %>', {people: people});
```

## Features:

1. Control flow with <% %>
2. Escaped output with <%= %> (escape function configurable)
3. Unescaped raw output with <%- %>
4. Newline-trim mode ('newline slurping') with -%> ending tag
5. Whitespace-trim mode (slurp all whitespace) for control flow with <%_ _%>
6. Custom delimiters (e.g. [? ?] instead of <% %>)
7. Includes
8. Client-side support
9. Static caching of intermediate JavaScript
10. Static caching of templates
11. Complies with the Express view system


* let talk about **Caching**

EJS ships with a basic in-process cache for caching the intermediate JavaScript functions used to render templates. It's easy to plug in LRU caching using Node's lru-cache library:
```
let ejs = require('ejs'),
    LRU = require('lru-cache');
ejs.cache = LRU(100); // LRU cache with 100-item limit
```
If you want to clear the EJS cache, call ejs.clearCache.