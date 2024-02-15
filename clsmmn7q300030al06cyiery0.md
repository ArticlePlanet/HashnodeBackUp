---
title: "How to Remove or Extract Metadata from Markdown Files in JavaScript"
datePublished: Fri Feb 02 2024 04:36:23 GMT+0000 (Coordinated Universal Time)
cuid: clsmmn7q300030al06cyiery0
slug: how-to-remove-or-extract-metadata-from-markdown-files-in-javascript

---

Title: **How to Remove or Extract Metadata from Markdown Files in JavaScript**

---
%[https://dev.to/sh20raj/parsemarkjs-a-lightweight-javascript-library-for-parsing-markdown-metadata-and-content-separately-1o6j]

---

## Introduction

Markdown files often contain metadata in the form of YAML front matter. This metadata provides additional information about the document, such as title, author, tags, and more. In certain scenarios, you may need to extract or remove this metadata programmatically using JavaScript. This article will guide you through the process of handling metadata in Markdown files.

## Removing Metadata from Markdown

If your goal is to remove the metadata section from a Markdown file, you can achieve this with a simple JavaScript function. Below is an example of how you can accomplish this:

```javascript
function removeMetadata(markdownContent) {
    const match = markdownContent.match(/^---([\s\S]*?)---([\s\S]*)/);

    if (match && match[2]) {
        return match[2].trim();
    }

    return markdownContent.trim();
}

const markdownWithMetadata = '---\ntitle: "Sample Markdown Document"\nauthor: John Doe\ndate: 2024-02-02\ntags:\n  - JavaScript\n  - Markdown\n---\n\n# Content\n\nThis is the content of the Markdown document.';

const markdownWithoutMetadata = removeMetadata(markdownWithMetadata);
console.log('Markdown without Metadata:', markdownWithoutMetadata);
```

In this example, the `removeMetadata` function uses a regular expression to identify and remove the YAML front matter. The resulting `markdownWithoutMetadata` variable will contain only the content of the Markdown file.

## Extracting Metadata from Markdown

Conversely, if you want to extract the metadata from a Markdown file, you can modify the function to capture the metadata as an object. Here's an example:

```javascript

function extractMetadata(markdown) {
        const frontMatter = markdown.split('---')[1];
        const metadataLines = frontMatter.split('\n').filter(line => line.trim() !== '');

        const metadata = {};
        metadataLines.forEach(line => {
            const [key, ...valueParts] = line.split(':').map(item => item.trim());
            metadata[key] = valueParts.join(':').replace(/(^"|"$)/g, '').trim();
        });

        // Convert tags to an array
        metadata.tags = metadata.tags ? metadata.tags.split(',').map(tag => tag.trim()) : [];

        return metadata;
    }

const markdownWithMetadata = '---\ntitle: "Sample Markdown Document"\nauthor: John Doe\ndate: 2024-02-02\ntags:\n  - JavaScript\n  - Markdown\n---\n\n# Content\n\nThis is the content of the Markdown document.';

const extractedMetadata = extractMetadata(markdownWithMetadata);
console.log('Extracted Metadata:', extractedMetadata);
```

In this example, the `extractMetadata` function creates an object `metadata` with key-value pairs based on the YAML front matter. The resulting `extractedMetadata` variable will contain the metadata as an object.

## Conclusion

Removing or extracting metadata from Markdown files in JavaScript can be achieved by leveraging regular expressions and string manipulation. Depending on your specific use case, you can choose between the provided examples to suit your needs. Feel free to adapt and extend the code to handle more complex scenarios or integrate it into your projects.