# dot
A simple dot language renderer

This is a basic html/js page, hosted on github pages that's meant to take dot language data from the url hash and display the resulting graph.
The rendering is done using the wonderful https://github.com/magjac/d3-graphviz library.

I made this page because most visual renderers are combined with dot language editors which didn't suit my needs.
It allows you to easily display graphs to your users. For example:
```javascript
const dot = 'digraph {a -> b}'
const encoded = encodeURIComponent(dot)
window.open(`https://ronyhe.github.io/dot/index.html?${encoded}`, '_blank')
```
