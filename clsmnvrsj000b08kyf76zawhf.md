---
title: "Top 50 Useful Regex Patterns"
datePublished: Tue Feb 13 2024 14:44:00 GMT+0000 (Coordinated Universal Time)
cuid: clsmnvrsj000b08kyf76zawhf
slug: top-50-useful-regex-patterns-1-1
canonical: https://codexdindia.blogspot.com/2024/02/top-50-useful-regex-patterns.html
cover: https://cdn.hashnode.com/res/hashnode/imageupload/v1707967718725/43e3f40f-327b-4d49-86ef-967a11ebbbd2.jpeg

---

**Title: Mastering Regular Expressions in JavaScript: Top 50 Useful Regex Patterns**

[![](https://cdn.hashnode.com/res/hashnode/imageupload/v1707967716030/24927713-2626-4998-b20e-4e393f2dfb86.jpeg)](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/hkjzg3sg1xr9cqk64d0t.jpeg)

**Introduction:**

Regular expressions (regex) are a powerful tool for pattern matching and text manipulation in JavaScript. Whether you're validating user input, extracting data from strings, or replacing text, regex can streamline your coding tasks. In this article, we'll explore 50 useful regex patterns that every JavaScript developer should know. These regex patterns cover a wide range of common scenarios, from validating email addresses to parsing URLs and beyond.

**1\. Validating Email Addresses:**

    const emailRegex = /^[\w-]+(\.[\w-]+)*@([\w-]+\.)+[a-zA-Z]{2,7}$/;
    

**2\. Validating URLs:**

    const urlRegex = /^(https?:\/\/)?([\da-z.-]+)\.([a-z.]{2,6})([/\w .-]*)*\/?$/;
    

**3\. Validating Dates in YYYY-MM-DD Format:**

    const dateRegex = /^\d{4}-\d{2}-\d{2}$/;
    

**4\. Validating Phone Numbers (US Format):**

    const phoneRegex = /^\(?(\d{3})\)?[- ]?(\d{3})[- ]?(\d{4})$/;
    

**5\. Validating Postal Codes (US Format):**

    const postalCodeRegex = /^\d{5}(?:-\d{4})?$/;
    

**6\. Validating Credit Card Numbers (Luhn Algorithm):**

    const creditCardRegex = /^(?:4[0-9]{12}(?:[0-9]{3})?|5[1-5][0-9]{14}|6(?:011|5[0-9][0-9])[0-9]{12}|3[47][0-9]{13}|3(?:0[0-5]|[68][0-9])[0-9]{11}|(?:2131|1800|35\d{3})\d{11})$/;
    

**7\. Validating Social Security Numbers (SSN):**

    const ssnRegex = /^\d{3}-\d{2}-\d{4}$/;
    

**8\. Validating IP Addresses (IPv4):**

    const ipRegex = /^(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$/;
    

**9\. Validating Hexadecimal Color Codes:**

    const hexColorRegex = /^#?([a-fA-F0-9]{6}|[a-fA-F0-9]{3})$/;
    

**10\. Extracting All URLs from a String:**

    const extractURLs = /https?:\/\/\S+/g;
    

**11\. Extracting All Email Addresses from a String:**

    const extractEmails = /[\w.-]+@[a-zA-Z-]+\.[a-zA-Z]{2,3}/g;
    

**12\. Matching HTML Tags:**

    const htmlTagsRegex = /<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)/gi;
    

**13\. Matching HTML Comments:**

    const htmlCommentsRegex = /<!--[\s\S]*?-->/g;
    

**14\. Matching CSS Classes:**

    const cssClassRegex = /\.([a-zA-Z_-][\w-]*)/g;
    

**15\. Matching Twitter Handles:**

    const twitterHandleRegex = /@[a-zA-Z0-9_]+/g;
    

**16\. Matching Hashtags:**

    const hashtagRegex = /#[a-zA-Z0-9_]+/g;
    

**17\. Matching Mentions in Tweets:**

    const mentionRegex = /@([a-zA-Z0-9_]+)/g;
    

**18\. Matching YouTube Video IDs in URLs:**

    const youtubeVideoIdRegex = /(?:https?:\/\/)?(?:www\.)?(?:youtube\.com\/(?:[^\/\n\s]+\/\S+\/|(?:v|e(?:mbed)?)\/|\S*?[?&]v=)|youtu\.be\/)([a-zA-Z0-9_-]{11})/;
    

**19\. Matching Twitter URLs:**

    const twitterUrlRegex = /(?:https?:\/\/)?(?:www\.)?twitter\.com\/(#!\/)?[a-zA-Z0-9_]+/;
    

**20\. Matching YouTube URLs:**

    const youtubeUrlRegex = /(?:https?:\/\/)?(?:www\.)?(?:youtube\.com\/(?:[^\/\n\s]+\/\S+\/|(?:v|e(?:mbed)?)\/|\S*?[?&]v=)|youtu\.be\/)([a-zA-Z0-9_-]{11})/;
    

**21\. Matching Instagram Usernames:**

    const instagramUsernameRegex = /(?:https?:\/\/)?(?:www\.)?instagram\.com\/[a-zA-Z0-9_]+/;
    

**22\. Matching Instagram URLs:**

    const instagramUrlRegex = /(?:https?:\/\/)?(?:www\.)?instagram\.com\/(p|tv|reel)\/[a-zA-Z0-9_]+/;
    

**23\. Matching YouTube Playlist URLs:**

    const youtubePlaylistRegex = /(?:https?:\/\/)?(?:www\.)?youtube\.com\/playlist\?list=([a-zA-Z0-9_-]+)/;
    

**24\. Matching Google Drive URLs:**

    const googleDriveUrlRegex = /(?:https?:\/\/)?drive\.google\.com\/(?:file\/d\/|open\?id=)([a-zA-Z0-9_-]+)/;
    

**25\. Matching SoundCloud URLs:**

    const soundcloudUrlRegex = /(?:https?:\/\/)?(?:www\.)?soundcloud\.com\/[a-zA-Z0-9_-]+\/[a-zA-Z0-9_-]+/;
    

**26\. Matching GitHub Repository URLs:**

    const githubRepoUrlRegex = /(?:https?:\/\/)?(?:www\.)?github\.com\/[a-zA-Z0-9_-]+\/[a-zA-Z0-9_-]+/;
    

**27\. Matching GitHub Gist URLs:**

    const githubGistUrlRegex = /(?:https?:\/\/)?(?:www\.)?gist\.github\.com\/[a-zA-Z0-9_-]+\/[a-zA-Z0-9]+/;
    

**28\. Matching Medium URLs:**

    const mediumUrlRegex = /(?:https?:\/\/)?(?:www\.)?medium\.com\/(@[a-zA-Z0-9_-]+)\/[a-zA-Z0-9_-]+/;
    

**29\. Matching Stack Overflow URLs:**

    const stackoverflowUrlRegex = /(?:https?:\/\/)?(?:www\.)?stackoverflow\.com\/questions\/([0-9]+)/;
    

**30\. Matching LinkedIn Profile URLs:**

    const linkedinProfileUrlRegex = /(?:https?:\/\/)?(?:www\.)?linkedin\.com\/in\/[a-zA-Z0-9_-]+/;
    

**31\. Matching IPv6 Addresses:**

    const ipv6Regex = /(?:(?:(?:[0-9a-fA-F]{1,4}:){6}|(?=(?:[0-9a-fA-F]{0,4}:){2,6}(?:[0-9.]{1,3})){((?=.*(::))(?=(.*?::))(::)?(([0-9a-fA-F]{1,4}:){0,5}|:)((?::[0-9a-fA-F]{1,4}){1,2}:|(?:[0-9]{1,3}\.){3}[0-9]{1,3})))(%.+)?\b/;
    

**32\. Matching Base64 Encoded Strings:**

    const base64Regex = /^[a-zA-Z0-9-_]+={0,2}$/;
    

**33\. Matching Markdown Headings:**

    const markdownHeadingRegex = /^(#{1,6})\s(.+)/;
    

**34\. Matching Markdown Links:**

    const markdownLinkRegex = /\[([^\]]+)\]\(([^)]+)\)/g;
    

**35\. Matching HTML Entities:**

    const htmlEntityRegex = /&(?:[a-zA-Z]+|#\d+);/;
    

**36\. Matching XML Tags:**

    const xmlTagRegex = /<([a-zA-Z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)/gi;
    

**37\. Matching Docker Image Tags:**

    const dockerTagRegex = /^[a-zA-Z0-9][a-zA-Z0-9._-]{0,127}$/;
    

**38\. Matching Semantic Versioning (SemVer):**

    const semverRegex = /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)(?:-((?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)?(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+([0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?$/;
    

**39\. Matching YAML Front Matter:**

    const yamlFrontMatterRegex = /---\n([\s\S]*?)\n---/;
    

**40\. Matching JSON Objects:**

    const jsonObjectRegex = /{[\s\S]*?}/;
    

**41\. Matching JSON Arrays:**

    const jsonArrayRegex = /\[[\s\S]*?\]/;
    

**42\. Matching CSS Color Codes:**

    const cssColorRegex = /#([0-9A-Fa-f]{6}|[0-9A-Fa-f]{3})/;
    

**43\. Matching HTML Hexadecimal Entities:**

    const htmlHexEntityRegex = /&#x[0-9A-Fa-f]+;/;
    

**44\. Matching HTML Decimal Entities:**

    const htmlDecimalEntityRegex = /&#\d+;/;
    

**45\. Matching Base64 Data URLs:**

    const base64DataUrlRegex = /^data:([a-z]+)\/([a-z]+);base64,([^\s]+)/;
    

**46\. Matching UUID (Universally Unique Identifier):**

    const uuidRegex = /^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[1-5][0-9a-fA-F]{3}-[89abAB][0-9a-fA-F]{3}-[0-9a-fA-F]{12}$/;
    

**47\. Matching ISBN (International Standard Book Number):**

    const isbnRegex = /^(?:ISBN(?:-10)?:? ?)?(?=[0-9X]{10}$|(?=(?:[0-9]+[- ]){3})[- 0-9X]{13}$|97[89][0-9]{10}$|(?=(?:[0-9]+[- ]){4})[- 0-9]{17}$)(?:97[89][- ]?)?[0-9]{1,5}[- ]?(?:[0-9]+[- ]?){2}[0-9X]$/;
    

**48\. Matching XML or HTML Comments:**

    const xmlHtmlCommentRegex = /<!--[\s\S]*?-->/;
    

**49\. Matching Google Analytics Tracking IDs:**

    const googleAnalyticsIdRegex = /^(UA|YT|MO)-\d{4,}-\d{1,2}$/;
    

**50\. Matching ISBN (International Standard Book Number) with Hyphens:**

    const isbnWithHyphensRegex = /^(?=(?:[0-9]+[- ]){3})[- 0-9]{13}$/;
    

**Conclusion:**

Regular expressions are an indispensable tool for working with text in JavaScript. By mastering these 50 useful regex patterns, you can handle a wide range of tasks efficiently, from validating user input to extracting data from strings and more. Experiment with these regex patterns in your projects and adapt them as needed to suit your specific requirements. Happy coding!