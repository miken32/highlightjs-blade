# highlightjs-blade
Syntax highlighting for Laravel Blade template files

## Usage

Simply include the Highlight.js library in your webpage or Node app, then load this module.

### Static website or simple usage

Simply load the module after loading Highlight.js.  You'll use the minified version found in the `dist` directory.  This module is just a CDN build of the language, so it will register itself as the Javascript is loaded.

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" src="/path/to/blade.min.js"></script>
<script type="text/javascript">
  hljs.highlightAll();
</script>
```

### With Node

If you're using Node, simply require the language module with `npm install miken32/highlightjs-blade`, then register it with Highlight.js.

```javascript
var hljs = require('highlight.js');
var hljsBlade = require('highlightjs-blade');

hljs.registerLanguage("blade", hljsBlade);
hljs.highlightAll();
```


## License

Highlight.js is released under version 2 of the GPL. See [LICENSE][1] file
for details.

### Author

Michael Newton <miken32@gmail.com>

[1]: https://github.com/miken32/highlightjs-blade/blob/master/LICENSE
