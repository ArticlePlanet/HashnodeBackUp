---
title: "How to Add a VS Code Editor to Your Website"
datePublished: Thu Oct 26 2023 13:28:55 GMT+0000 (Coordinated Universal Time)
cuid: cls2rp5mr00040ajkajro6zd7
slug: how-to-add-a-vs-code-editor-to-your-website

---

# How to Add a VS Code Editor to Your Website

The Monaco editor by Microsoft provides a code editor component that can be easily integrated into websites. With just a few lines of code, you can add a full-featured editor similar to VS Code in your web app. In this tutorial, we'll see how to do just that.

## Getting Started

To use Monaco, we need to include it in our page. We can get it from a CDN:

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.23.0/min/vs/loader.min.js"></script>
```

This will load the Monaco library asynchronously. Next, we need a `<div>` in our HTML where we can instantiate the editor:

```html
<div id="editor"></div>
```

Now in our JavaScript code, we can initialize Monaco and create the editor:

```js
require.config({ paths: { 'vs': 'https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.23.0/min/vs' }});

require(["vs/editor/editor.main"], function() {
  const editor = monaco.editor.create(document.getElementById('editor'), {
    value: ['<!DOCTYPE html>',
             '<html>',
             '  <body>',
             '    <h1>Hello World!</h1>', 
             '  </body>',
             '</html>'].join('\n'),
    language: 'html'
  });
}); 
```

This will create the editor with some sample HTML content.

## Adding Theme

To make it look like VS Code, we need to add the theme CSS:

```html
<link href="https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.23.0/min/vs/editor/editor.main.css" rel="stylesheet" /> 
```

The `editor.main.css` provides the core editor styles. For the VS Code dark theme, include:

```js
const editor = monaco.editor.create(..., {
  theme: 'vs-dark' 
});
```

That's it! We now have a VS Code-like editor on our page.

## Configuring Languages

To add language support, pass the `language` parameter when creating the editor:

```js
const editor = monaco.editor.create(..., {
  language: 'javascript'
}); 
```

Monaco comes with intelligent code completion, syntax highlighting, and validation for popular languages like HTML, CSS, JavaScript and more.

## Conclusion

With just a few lines of code, Monaco makes it easy to integrate a code editor into your web app. Customizable themes and language support takes it to the next level providing a full-featured coding environment for your users.

Let me know if you would like me to expand or modify anything in this article!