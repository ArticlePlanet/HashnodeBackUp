---
title: "ParseMark.js - A lightweight JavaScript library for parsing Markdown metadata and content separately"
datePublished: Fri Feb 02 2024 10:09:40 GMT+0000 (Coordinated Universal Time)
cuid: clsmmn3ex000e09ide68k1gyi
slug: parsemarkjs-a-lightweight-javascript-library-for-parsing-markdown-metadata-and-content-separately

---


# ParseMark.js

A lightweight JavaScript library for parsing Markdown metadata and content separately

[![License](https://cdn.hashnode.com/res/hashnode/image/upload/v1707965634744/87dc0453-bf7d-4131-89b5-f7e5fa39dd2b.svg)](https://opensource.org/licenses/MIT)

%[https://github.com/SH20RAJ/ParseMark/]

## Installation

### Using npm

```bash
npm install parsemarkjs
```

### Using CDN

Include the following script tag in your HTML file:

```html
<script src="https://cdn.jsdelivr.net/gh/SH20RAJ/ParseMark@main/ParseMark.js"></script>
```

## Usage

### Constructor

```javascript
const markdown = `
---
title: "Sample Post"
tags: javascript, library, markdown
datePublished: Fri, 04 Feb 2024 12:00:00 GMT
---

# Sample Post

This is a sample post content.
`;

const parser = new ParseMark(markdown);
```

### getMetadata()

```javascript
const metadata = parser.getMetadata();
console.log('Metadata:', metadata);
```

### getRawMetadata()

```javascript
const rawMetadata = parser.getRawMetadata();
console.log('Raw Metadata:', rawMetadata);
```

### getContent()

```javascript
const content = parser.getContent();
console.log('Content:', content);
```

#### Example Output

<img width="577" alt="Screenshot 2024-02-02 at 3 14 25 PM" src="https://github.com/SH20RAJ/ParseMark/assets/66713844/d1b845b1-2ae7-4d07-89ad-b60006e22165">

