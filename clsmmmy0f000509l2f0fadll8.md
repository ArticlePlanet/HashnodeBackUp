---
title: "Code/Syntax Highlighting Using highlight.js - Displaying Code on Website/Blogger with jsDelivr CDN"
datePublished: Sat Feb 03 2024 14:14:19 GMT+0000 (Coordinated Universal Time)
cuid: clsmmmy0f000509l2f0fadll8
slug: codesyntax-highlighting-using-highlightjs-displaying-code-on-websiteblogger-with-jsdelivr-cdn

---



## Code/Syntax Highlighting Using highlight.js - Displaying Code on Website/Blogger with jsDelivr CDN


> Get More Theming Options [Here](https://www.jsdelivr.com/package/npm/highlight.js?path=styles&tab=files) :- https://codexdindia.blogspot.com/2022/01/code-or-syntax-highlighting-using-highlightjs.html


**Introduction:**
Code highlighting plays a crucial role in creating visually appealing and developer-friendly websites. In this article, we'll explore how to implement code or syntax highlighting using the powerful Highlight.js library and leverage the jsDelivr CDN for seamless integration on your website or Blogger platform.

### Step 1: Obtain Highlight.js from jsDelivr CDN

Start by including Highlight.js directly from the jsDelivr CDN in your HTML file. Omitting the version ensures you always get the latest one.

```html
<!-- Include Highlight.js from jsDelivr CDN -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/highlight.js/styles/default.min.css">
<script src="https://cdn.jsdelivr.net/npm/highlight.js/lib/index.min.js"></script>
```

### Step 2: Initialize Highlight.js

Initialize Highlight.js by calling the `initHighlightingOnLoad()` function within a script tag.

```html
<script>
  document.addEventListener('DOMContentLoaded', (event) => {
    hljs.initHighlightingOnLoad();
  });
</script>
```

This ensures that code highlighting is applied once the document is fully loaded.

### Step 3: Mark Up Your Code Snippets

Wrap your code snippets inside `<pre><code>` tags and add a class indicating the programming language. Highlight.js will automatically detect the language based on the specified class.

```html
<pre><code class="javascript">
  // Your JavaScript code here
</code></pre>
```

### Step 4: Apply a Theme (Optional)

Highlight.js comes with a variety of themes. Apply a theme by including the corresponding stylesheet from jsDelivr CDN. For example, using the 'monokai' theme:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/highlight.js/styles/monokai.min.css">
```

### Step 5: Switching Themes

You can easily switch themes by replacing the theme CDN link. For instance, to switch to the 'night-owl' theme:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/highlight.js/styles/night-owl.min.css">
```

Explore the full list of themes [here](https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/). Replace the theme name in the CDN link accordingly.

### Step 6: Additional Features

Highlight.js offers additional features, such as line numbering. To enable line numbers, modify the `<pre>` tag:

```html
<pre><code class="javascript hljs" data-line-numbers>
  // Your JavaScript code here
</code></pre>
```

Explore the Highlight.js documentation for more customization options.

### Step 7: Displaying Code on Blogger

If you're using Blogger, navigate to the HTML editor and insert your highlighted code within the `<pre>` tags with the specified language class.

**Conclusion:**
By following these steps and leveraging jsDelivr CDN, you can easily implement code or syntax highlighting on your website or Blogger platform. This enhances the readability of your code snippets, making your content more engaging and accessible to developers and readers alike.