---
title: "How to Use Git with Hugging Face: From Cloning to Pushing with Access Token Verification"
datePublished: Sat Oct 14 2023 11:20:45 GMT+0000 (Coordinated Universal Time)
cuid: cls2rpfvd000008jq6wc6hchn
slug: how-to-use-git-with-hugging-face-from-cloning-to-pushing-with-access-token-verification
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1706764819120/72298af2-48e5-46fb-9208-fe54909efd31.png

---


# How to Use Git with Hugging Face: From Cloning to Pushing with Access Token Verification

Hugging Face is a popular platform for machine learning, natural language processing (NLP), and deep learning models. It provides a wide range of pre-trained models and tools for collaborative development. Git integration is a crucial part of working on projects with Hugging Face, and with recent changes in authentication methods, it's important to understand how to use Git seamlessly with the platform. This guide will take you through the entire process, from cloning a repository to committing changes and pushing them, all while ensuring proper access token verification.

## Prerequisites

Before you start, make sure you have the following prerequisites:

1. A Hugging Face account: You'll need a Hugging Face account to access your repositories.

2. Git installed: Ensure that Git is installed on your local machine. You can download it from [https://git-scm.com/](https://git-scm.com/).

3. A personal access token (PAT): To interact with Hugging Face's Git repositories, you need a personal access token. You can create one in your Hugging Face settings, as discussed below.

## Step 1: Creating a Personal Access Token (PAT)

1. Log in to your Hugging Face account.

2. Go to your account settings by clicking on your profile picture and selecting "Settings" from the dropdown menu.

3. In the "Tokens" section, click on "New token."

4. Provide a name for your token and select the necessary scopes. For Git operations, you'll need the "Git" scope. Optionally, you can also select other scopes based on your requirements.

5. Click "Create" to generate your access token. Make sure to save it in a safe place, as you won't be able to view it again.

## Step 2: Cloning a Repository

Now that you have your access token, you can start working with Git and Hugging Face repositories.

1. Open your terminal or Git client.

2. Navigate to the directory where you want to clone the repository.

3. Use the following command to clone a Hugging Face repository, replacing `USERNAME` with your Hugging Face username, `REPO_NAME` with the repository name, and `YOUR_ACCESS_TOKEN` with the personal access token you generated:

   ```shell
   git clone https://USERNAME:YOUR_ACCESS_TOKEN@huggingface.co/spaces/USERNAME/REPO_NAME.git
   ```

4. The repository will be cloned to your local machine.

## Step 3: Setting the Git Remote URL

To ensure your access token is configured correctly, set the Git remote URL:

1. Navigate to the cloned repository:

   ```shell
   cd REPO_NAME
   ```

2. Use the following command to set the Git remote URL, replacing `YOUR_ACCESS_TOKEN` with your personal access token:

   ```shell
   git remote set-url origin https://USERNAME:YOUR_ACCESS_TOKEN@huggingface.co/spaces/USERNAME/REPO_NAME.git
   ```

3. This step ensures that your access token is used for authentication when you interact with the repository.

## Step 4: Making Changes

With the repository cloned and the remote URL set, you can now make changes to your project.

1. Create, modify, or delete files in your project as needed.

2. Use Git commands to stage and commit your changes. For example:

   ```shell
   git add .
   git commit -m "Your commit message"
   ```

## Step 5: Pushing Changes

Once you've committed your changes, you can push them to the Hugging Face repository.

1. Use the following command to push your changes:

   ```shell
   git push
   ```

   Your access token will be used for authentication, and you won't be prompted for a password.

2. Your changes will be pushed to the Hugging Face repository.

## Step 6: Access Token Verification

It's important to keep your access token secure. Do not share it with others or expose it in public repositories. If your access token is compromised or needs to be regenerated for any reason, you can do so in your Hugging Face settings.

## Conclusion

Using Git with Hugging Face is essential for collaborative machine learning and NLP projects. With the recent changes in authentication, it's crucial to understand how to use a personal access token for secure and seamless interaction with Git repositories on the platform. By following this guide, you can clone, make changes, commit, and push your code while keeping your access token secure and your workflow efficient. Happy coding!