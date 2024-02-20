---
title: "Create Telegram Bot - NextJS and Hosting on Vercel - Free"
datePublished: Tue Feb 20 2024 10:08:39 GMT+0000 (Coordinated Universal Time)
cuid: clsu7desf000h08ld8kh7fqzn
slug: create-telegram-bot-nextjs-and-hosting-on-vercel-free
canonical: https://codexdindia.blogspot.com/2024/02/create-telegram-bot-nextjs-and-hosting.html

---

### Create Telegram Bot - NextJS and Hosting on Vercel - Free

Title: Building a Telegram Bot with Next.js, GitHub, and Vercel

Creating a Telegram bot with Next.js and deploying it on Vercel is a great way to build interactive bots quickly. In this tutorial, we'll take it a step further by organizing our project structure and enabling deployment through GitHub and Vercel's user-friendly UI.

### [](https://codexdindia.blogspot.com/2024/02/create-telegram-bot-nextjs-and-hosting.html#prerequisites)Prerequisites:

*   Basic knowledge of JavaScript and Node.js
*   Understanding of REST APIs and webhook concepts
*   Telegram account
*   GitHub account
*   Vercel account

### [](https://codexdindia.blogspot.com/2024/02/create-telegram-bot-nextjs-and-hosting.html#step-1-set-up-telegram-bot)Step 1: Set up Telegram Bot

1.  Create a new bot on Telegram using BotFather and obtain the bot token.

### [](https://codexdindia.blogspot.com/2024/02/create-telegram-bot-nextjs-and-hosting.html#step-2-initialize-a-nextjs-project)Step 2: Initialize a Next.js Project

1.  Install Node.js if you haven't already.
2.  Initialize a new Next.js project:

     npx create-next-app my-telegram-bot
    

Enter fullscreen mode Exit fullscreen mode

1.  Navigate to your project directory:

     cd my-telegram-bot
    

Enter fullscreen mode Exit fullscreen mode

### [](https://codexdindia.blogspot.com/2024/02/create-telegram-bot-nextjs-and-hosting.html#step-3-organize-project-structure)Step 3: Organize Project Structure

1.  Create a folder named `src` in your project directory.
2.  Inside the `src` folder, create a folder named `api`.
3.  Inside the `api` folder, create a file named `telegram.js`.

### [](https://codexdindia.blogspot.com/2024/02/create-telegram-bot-nextjs-and-hosting.html#step-4-write-telegram-bot-code)Step 4: Write Telegram Bot Code

1.  Open `src/api/telegram.js` and add the following code:

     import { Telegraf } from 'telegraf';
     const bot = new Telegraf(process.env.TELEGRAM_BOT_TOKEN);
     bot.on('text', (ctx) => {
     ctx.reply('Hello! You said: ' + ctx.message.text);
     });
     bot.telegram.setWebhook(`https://${process.env.VERCEL_URL}/api/telegram`);
     export default async (req, res) => {
     await bot.handleUpdate(req.body, res);
     };
    

Enter fullscreen mode Exit fullscreen mode

### [](https://codexdindia.blogspot.com/2024/02/create-telegram-bot-nextjs-and-hosting.html#step-5-deploy-to-github)Step 5: Deploy to GitHub

1.  Initialize a git repository in your project directory:

     git init
    

Enter fullscreen mode Exit fullscreen mode

1.  Add your files to the repository and commit:

     git add .
     git commit -m "Initial commit"
    

Enter fullscreen mode Exit fullscreen mode

1.  Create a new repository on GitHub.
2.  Link your local repository to the remote GitHub repository:

     git remote add origin <GitHub repository URL>
    

Enter fullscreen mode Exit fullscreen mode

1.  Push your code to GitHub:

     git push -u origin main
    

Enter fullscreen mode Exit fullscreen mode

### [](https://codexdindia.blogspot.com/2024/02/create-telegram-bot-nextjs-and-hosting.html#step-6-deploy-to-vercel)Step 6: Deploy to Vercel

1.  Sign in to your Vercel account.
2.  Import your project from GitHub.
3.  Follow the prompts to deploy your project.
4.  Set the environment variable `TELEGRAM_BOT_TOKEN` to your bot token in the Vercel dashboard.

### [](https://codexdindia.blogspot.com/2024/02/create-telegram-bot-nextjs-and-hosting.html#step-7-set-webhook-url)Step 7: Set Webhook URL

1.  Use curl or any other method to set the webhook URL to your current page `api/telegram.js`:

     curl -F "url=https://your-vercel-url.vercel.app/api/telegram" https://api.telegram.org/bot<YOUR_BOT_TOKEN>/setWebhook
    

Enter fullscreen mode Exit fullscreen mode

Replace `your-vercel-url` with your Vercel project URL and `<YOUR_BOT_TOKEN>` with your actual bot token.

### [](https://codexdindia.blogspot.com/2024/02/create-telegram-bot-nextjs-and-hosting.html#step-8-test-your-telegram-bot)Step 8: Test Your Telegram Bot

1.  Start a conversation with your bot on Telegram.
2.  Send a message, and you should receive a response from your bot echoing your message.

Congratulations! You've successfully created a Telegram bot using Next.js, organized your project structure, deployed it on GitHub and Vercel, and set up the webhook for message handling. You can now further customize your bot's functionality and interaction based on your requirements.