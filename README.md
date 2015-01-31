HTML Text Editor Plugin
=======================

As mentioned in the title above.

> This is a HTML version of the previous plugin called [MTE](https://github.com/tovic/markdown-text-editor "MTE &ndash; Markdown Text Editor").

Demo
----

&rarr; http://rawgit.com/tovic/html-text-editor/master/index.html

Basic Usage
-----------

Place the icon fonts and the CSS file in the head:

``` .html
<link href="css/font-awesome.css" rel="stylesheet">
<link href="css/style.css" rel="stylesheet">
```

Create a textarea element in the body:

``` .html
<textarea></textarea>
```

Place the library and the editor plugin after the `<textarea>` element then execute the plugin:

``` .html
<script src="js/library.js"></script>
<script src="js/hte.js"></script>
<script>
var myEditor = new HTE(document.getElementsByTagName('textarea')[0]);
</script>
```

Options
-------

Just like the **MTE** plugin but initiated by `HTE` instead of `MTE`:

``` .javascript
var myEditor = new HTE(elem, { ... });
myEditor.button('foo', {
    title: 'Bar',
    click: function() {
        alert('Baz!');
    }
});
```

Read more on the [Wiki Pages of MTE Plugin](https://github.com/tovic/markdown-text-editor/wiki)

Extra Options
-------------

| Option | Usage | Example |
| ------ | ----- | ------- |
| `emptyElementSuffix` | Used to determine the end character of self-closing HTML tags. | ` />` |
| `autoEncodeHTML` | Automatically encode the selected HTML string inside `<code>` element? | `true` |