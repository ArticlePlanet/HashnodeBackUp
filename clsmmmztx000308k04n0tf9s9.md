---
title: "GitCodeEmbedder - Free Embedder of GitHub Repo To Your Website / Blog"
datePublished: Sat Feb 03 2024 13:22:32 GMT+0000 (Coordinated Universal Time)
cuid: clsmmmztx000308k04n0tf9s9
slug: gitcodeembedder-free-embedder-of-github-repo-to-your-website-blog

---

# GitCodeEmbedder: Embed GitHub Repositories Easily on Your Website

In the fast-paced world of web development, sharing code snippets, examples, or even entire repositories has become a common practice. GitHub serves as a popular platform for hosting code, and developers often want to showcase their work directly on their websites or blogs. This is where GitCodeEmbedder comes into play, offering a simple and efficient solution to embed GitHub repositories seamlessly.

## What is GitCodeEmbedder?

GitCodeEmbedder is a free tool that allows you to embed GitHub repositories directly onto your website or blog. Whether you want to showcase a specific file, a collection of files, or even an entire repository, GitCodeEmbedder simplifies the process by providing an easy-to-use iframe code snippet.

## Getting Started

To use GitCodeEmbedder, follow these simple steps:

1. Visit the [GitCodeEmbedder website](https://gitcodeembedder.blogspot.com/) - https://gitcodeembedder.blogspot.com/.

2. Copy the provided iframe code snippet.

3. Paste the code into your website or blog, making sure to customize the `src` attribute of the iframe with your GitHub repository details.

   ```html
   <iframe src="https://gitcodeembedder.blogspot.com/?gh=[User]/[Repo]/main/[File Url]" width="100%" height="700px" frameborder="0"></iframe>
   ```

4. Customize further using optional URL attributes:
   - To embed files from a URL instead of GitHub, use `?url=[YourFileUrl]`.
   - Set the language of the file using `&lang=[languageName]`.
   - Display a single line of HTML using `&html=[YourOneLineHTML]`.
   - Embed an entire GitHub repository using `?gh=[User]/[Repo]/main`.

## Additional Features

### Embedding from URL

GitCodeEmbedder supports embedding files directly from a URL. This is useful if your code or file is hosted elsewhere. Use the `?url=` attribute followed by the file URL.

Example:
```html
?url=https://cdnjs.cloudflare.com/ajax/libs/mediaelement/4.2.6/mediaelementplayer.css&lang=css
```

### Setting Language

Specify the language of the embedded file using the `&lang=` attribute.

Example:
```html
?gh=SH20RAJ/YouTubeTitleUpdate/main/Code.gs&lang=javascript
```

### Single Line HTML

If you want to display a single line of HTML, use the `&html=` attribute.

Example:
```html
?html=<h1>GitCodeEmbedder - Free Embedder of GitHub Repo To Your Website / Blog</h1>
```

### Embedding GitHub Repository

To embed an a GitHub repository file, use the `?gh=` attribute followed by the repository details.

Example:
```html
?gh=CDNsFree2/DirecJS/main/DirecJS.js
```
https://gitcodeembedder.blogspot.com/?gh=cdnsfree2/DirecJS/main/DirecJS.js&lang=javascript


## Conclusion

GitCodeEmbedder streamlines the process of showcasing your GitHub repositories on your website. With its user-friendly approach and additional customization options, developers can seamlessly integrate their code into their online presence. Whether you're a blogger, developer, or both, GitCodeEmbedder is a handy tool for sharing your code with the world. Try it out and enhance your website with embedded GitHub repositories today!