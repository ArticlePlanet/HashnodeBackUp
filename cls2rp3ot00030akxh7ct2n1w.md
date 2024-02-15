---
title: "Google Docs Viewer - view/embed various file types directly in their BROWSER without the need for downloading"
datePublished: Fri Jan 05 2024 12:31:28 GMT+0000 (Coordinated Universal Time)
cuid: cls2rp3ot00030akxh7ct2n1w
slug: google-docs-viewer-viewembed-various-file-types-directly-in-their-browser-without-the-need-for-downloading

---

Title: A Guide to Using Google Docs Viewer for Seamless File Viewing

Introduction:
Google Docs Viewer is a convenient tool provided by Google that allows users to view various file types directly in their web browsers without the need for downloading. This feature is particularly handy when you want to quickly review a document, presentation, or spreadsheet without the hassle of saving it to your device. In this article, we'll explore how to use Google Docs Viewer and the supported file types.

%[https://codepen.io/SH20RAJ/pen/mdoVNrP]


### Step 1: Obtain the File URL

Before using Google Docs Viewer, you need the URL of the file you want to view. This can be a Google Docs, Sheets, Slides, or any other supported file hosted on the web. Ensure that the file is shared with the appropriate permissions to allow viewing.

### Step 2: Formulate the Google Docs Viewer URL

Once you have the file URL, you'll need to create a new URL for Google Docs Viewer. Append the original file URL to the following link:

```
https://docs.google.com/gview?url=
```

For example, if your file URL is `https://example.com/document.pdf`, the Google Docs Viewer URL would be:

```
https://docs.google.com/gview?url=https://example.com/document.pdf
```

For embedding use parameter `&embedded=true` in the URL.
### Step 3: Open the Google Docs Viewer URL

Enter the generated Google Docs Viewer URL into your web browser and press Enter. Google Docs Viewer will then load the file, displaying it directly in your browser window.

### Supported File Types:

Google Docs Viewer supports a variety of file types, including but not limited to:

1. **Documents:**
   - Google Docs (doc, docx)
   - PDF (pdf)
   - Text Documents (txt)

2. **Spreadsheets:**
   - Google Sheets (xls, xlsx)
   - Comma-Separated Values (csv)

3. **Presentations:**
   - Google Slides (ppt, pptx)
   - Microsoft PowerPoint (pps, ppt)

### Tips and Considerations:

- **Share Permissions:** Ensure that the file you want to view is shared with the appropriate permissions. Google Docs Viewer won't be able to display files that are not accessible to the viewer.

- **Browser Compatibility:** Google Docs Viewer is compatible with most modern web browsers, including Chrome, Firefox, Safari, and Edge. Ensure that your browser is up to date for optimal performance.

- **Internet Connection:** As Google Docs Viewer fetches the file from the web, a stable internet connection is necessary for seamless viewing.

By following these simple steps, you can leverage Google Docs Viewer to quickly preview and review various file types directly in your browser, eliminating the need to download files for a brief examination.

Sample Links for Testing :-

| File Type | File Link | Google Docs Viewer URL |
|-----------|-----------|-------------------------|
| PDF       | https://www.africau.edu/images/default/sample.pdf | https://docs.google.com/gview?url=https://www.africau.edu/images/default/sample.pdf               |
| TXT       | https://www.w3.org/TR/2003/REC-PNG-20031110/iso_8859-1.txt | https://docs.google.com/gview?url=https://www.w3.org/TR/2003/REC-PNG-20031110/iso_8859-1.txt |
| XLS       | https://filesamples.com/samples/document/xls/sample3.xls | https://docs.google.com/gview?url=https://filesamples.com/samples/document/xls/sample3.xls |
| PPT       | https://scholar.harvard.edu/files/torman_personal/files/samplepptx.pptx | https://docs.google.com/gview?url=https://scholar.harvard.edu/files/torman_personal/files/samplepptx.pptx               |
| CSV       | https://media.githubusercontent.com/media/datablist/sample-csv-files/main/files/customers/customers-100.csv | https://docs.google.com/gview?url=https://media.githubusercontent.com/media/datablist/sample-csv-files/main/files/customers/customers-100.csv               |

%[https://codepen.io/SH20RAJ/pen/qBvbeEG ]

