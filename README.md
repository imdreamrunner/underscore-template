# Template Engine from Underscore.js

The template engine from underscore.js is tiny but easy to use.
If you don't want to use the whole underscore.js library but need
a tiny, elegant template engine, please consider this project.

## How to use

### Download the library

* [Uncompressed Version](https://github.com/imdreamrunner/underscore-template/raw/master/underscore-template.js)
* [Production Version](https://github.com/imdreamrunner/underscore-template/raw/master/underscore-template.min.js)

### Include the library

```html
<script type="application/javascript" src="/path/to/underscore-template.min.js"></script>
```

### Usage

(Copy from underscore.js)

Compiles JavaScript templates into functions that can be evaluated for rendering. Useful for rendering complicated bits of HTML from JSON data sources. Template functions can both interpolate variables, using `<%= … %>`, as well as execute arbitrary JavaScript code, with `<% … %>`. If you wish to interpolate a value, and have it be HTML-escaped, use `<%- … %>` When you evaluate a template function, pass in a data object that has properties corresponding to the template's free variables.

```javascript
var compiled = _template("hello: <%= name %>");
compiled({name: 'moe'});
=> "hello: moe"

var template = _template("<b><%- value %></b>");
template({value: '<script>'});
=> "<b>&lt;script&gt;</b>"
```

## Copyright & License

The template engine is extracted from underscore.js, and necessary
modification is done.

It is open-sourced and released under the same license as underscore.js.
