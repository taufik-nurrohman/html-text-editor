HTML Text Editor Plugin
=======================

As mentioned in the title above.

> This is the HTML version of the previous plugin called [MTE](https://github.com/tovic/markdown-text-editor "MTE – Markdown Text Editor").

Demo
----

![html-text-editor](https://f.cloud.github.com/assets/1669261/2492943/8db3fa4e-b26a-11e3-8d5e-823c8d594b64.png)

→ https://rawgit.com/tovic/html-text-editor/master/index.html

Basic Usage
-----------

Put icon fonts and CSS files in the `<head>`:

~~~ .html
<link href="css/font-awesome.min.css" rel="stylesheet">
<link href="css/hte.min.css" rel="stylesheet">
~~~

Create a `<textarea>` element in the body:

~~~ .html
<textarea></textarea>
~~~

Put editor and **HTE** plugin after the `<textarea>` element then execute the plugin:

~~~ .html
<script src="js/editor.min.js"></script>
<script src="js/hte.min.js"></script>
<script>
var myEditor = new HTE(document.getElementsByTagName('textarea')[0]);
</script>
~~~

Options
-------

Just like the **MTE** plugin but initiated by `HTE` instead of `MTE`:

~~~ .javascript
var myEditor = new HTE(elem, { ... });
myEditor.button('foo', {
    title: 'Bar',
    click: function() {
        alert('Baz!');
    }
});
~~~

Read more on the [MTE Wiki Pages](https://github.com/tovic/markdown-text-editor/wiki)

Extra Options
-------------

| Option | Usage | Example |
| ------ | ----- | ------- |
| `autoEncodeHTML` | Automatically encode the selected HTML string inside `<code>` element? | `true` |