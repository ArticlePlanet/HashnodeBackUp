---
title: "Upload files to a Hugging Face space using the CLI and Python, including remote file uploads"
datePublished: Tue Oct 17 2023 09:33:00 GMT+0000 (Coordinated Universal Time)
cuid: cls2rpbd2000009jnh2pigo4n
slug: upload-files-to-a-hugging-face-space-using-the-cli-and-python-including-remote-file-uploads

---

How to upload files to a Hugging Face space using the CLI and Python, including remote file uploads:

# Uploading Files to Hugging Face Spaces

Hugging Face Spaces allow you to easily host models and apps. A key part of managing a Space is uploading files - like datasets, model files, images, etc. Here are some tips on how to upload files to your Space using the Hugging Face CLI and Python library.

## Uploading Local Files

To upload a local file to your Space from the command line, use the `huggingface-cli upload` command:

```
huggingface-cli upload username/my-space ./local/file.txt
```

This will upload `file.txt` directly to the root of your Space. You can also specify a path within the Space:

```
huggingface-cli upload username/my-space ./local/data.csv data/data.csv 
```

In Python, install the `huggingface_hub` library and use `upload_file()`:

```python
from huggingface_hub import login, upload_file

login(token="YOUR_TOKEN")

upload_file(
  path_or_fileobj="./local/image.png",
  path_in_repo="images/profile.png",
  repo_id="username/my-space"
)
```

You can upload entire folders using `upload_folder()` instead.

## Uploading Remote Files 

To upload a file from a URL to your Space, you can use the `huggingface-cli` with the `--remote` flag:

```
huggingface-cli upload username/my-space --remote https://example.com/data.csv
```

This will download the file and upload it. In Python, you can use the `requests` library:

```python
import requests
from huggingface_hub import login, upload_file

url = "https://example.com/file.txt"

# Download file
response = requests.get(url)
contents = response.content

login(token="YOUR_TOKEN") 

upload_file(
  path_or_fileobj=contents,
  path_in_repo="remote_data.txt",
  repo_id="username/my-space"  
)
```

This way you can download a remote file and directly upload the contents to your Space in one step.

## Summary

Key points:

- Use `huggingface-cli upload` to upload local files and folders 
- Pass `--remote` to upload directly from a URL
- In Python, use `upload_file()` and `upload_folder()` from `huggingface_hub`
- Download remote files first before uploading the contents

This provides some handy code snippets to easily manage files in your Hugging Face Spaces!