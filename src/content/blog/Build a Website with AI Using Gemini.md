---
title: 'Build a Website with AI: Go Live Using Gemini, VS Code, GitHub & Vercel'
description: 'Learn how to build a website with AI using Gemini, VS Code, GitHub, and Vercel. Copy, paste, and launch your site with this beginner-friendly project.'
pubDate: 'Oct 05 2026'
heroImage: 'https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=1600&q=80'
category: 'Projects'
isPopular: false
---

> **Disclosure:** Some links in this post are affiliate links. If you sign up through them, we may earn a commission at no extra cost to you.

You don't have to be a web developer to build a website. With the right AI prompt, the workflow is mostly copy, paste, and save.

In this project, you'll build a complete, responsive website from scratch using four tools: **VS Code**, **Gemini**, **GitHub**, and **Vercel**. By the end, your site will be live on the internet, and you can connect your own domain name.

Prefer watching? Here's the full video walkthrough:

<div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;">
  <iframe
    src="https://www.youtube.com/embed/2If8AywYx-o"
    title="Build a Website with AI: Go Live Using Gemini, VS Code, GitHub & Vercel"
    style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
</div>

## What You'll Build and the Tools You Need

The demo project is a music artist website with a modern glassmorphic design, a working audio player, and a booking form. The same workflow works for an NGO, a digital marketing agency, a portfolio, or any business site.

Because this is a front-end website, you don't need a back end. That keeps the setup simple and the hosting straightforward.

Here are the four tools and what each one does:

- **[VS Code](https://code.visualstudio.com/Download?_exp_download=fb315fc982)** is the text editor where you paste and save your code.
- **[Gemini](https://gemini.google.com)** is the AI assistant that writes the code and guides you step by step.
- **[GitHub](https://github.com)** stores your website files in a repository (think of it as a container).
- **[Vercel](https://vercel.com)** hosts your site and puts it online.

> **Pro Tip:** You can use any text editor, even Notepad. VS Code is recommended because it makes working with multiple files much easier.

## Step 1: Install VS Code

1. Go to the VS Code download page.
2. Choose your system: Windows, Debian/Ubuntu (.deb), Red Hat/Fedora/SUSE (.rpm), or Mac.
3. Run the installer and follow the prompts.

## Step 2: Prompt Gemini to Guide You

The quality of your website depends on your prompt. This one tells the AI to act like an expert developer, explain every step, and label which file each piece of code belongs to.

Copy this prompt, then replace the bracketed parts with your own details:

```text
You are an expert web developer with 10 years of professional experience. Your task is to guide me step by step in building a professional website for my [type of website, e.g. music career, NGO, digital marketing agency] using HTML, CSS, and JavaScript.

My brand name is [your brand name].

Guide me through every stage of the development process, starting from planning and setting up the project to designing, coding, testing, and launching the website.

For each stage, explain what we are doing and why. Provide clear, step-by-step instructions. Provide the complete code I need to copy and paste. Clearly indicate which file each piece of code belongs to, whether it's HTML, CSS, or JavaScript.

Keep the code beginner-friendly and explain important parts when necessary. Do not skip steps or assume that I already know how to do something.

Build the website progressively, one stage at a time. Wait for my confirmation before moving to the next major stage.
```

Open Gemini, paste the prompt, and select the **Pro** model before sending. The Pro model has stronger reasoning, which usually means better code than the faster, lighter models.

> **Pro Tip:** Read every instruction the AI gives you before following it. If you understand what each step does, you can steer the AI toward exactly what you want.

## Step 3: Create Your Project Folder and Files

Follow Gemini's first instructions to set up your workspace:

1. Create a new folder on your desktop, such as `my-website`.
2. Open VS Code and go to **File > Open Folder**.
3. Select the folder you just created.
4. Create three empty files using the **New File** icon:
   - `index.html` defines the structure (menu, sections, footer).
   - `style.css` controls the design and look.
   - `script.js` handles interactivity such as the mobile menu, animations, and the audio player.

Paste Gemini's starter code into `index.html`, save with **Ctrl + S**, then double-click the file in your folder. It should open in your browser and show a welcome message. That confirms your foundation works.

## Step 4: Ask for the Complete Code

By default, the AI may build the site feature by feature across many stages. That can be slow and confusing for beginners.

Send a follow-up instruction like this:

```text
Don't build it by features. Provide the complete code for the whole website in separate files: index.html, style.css, and script.js.
```

Gemini may first return everything in a single file with a live preview. If so, ask it to split the code into three files. Then:

1. Copy the HTML into `index.html`, select all, paste, and save.
2. Copy the CSS into `style.css` and save.
3. Copy the JavaScript into `script.js` and save.
4. Refresh your browser and test everything: the mobile menu, audio player, forms, and section links.

> **Pro Tip:** To add things later, like new songs, events, or tour dates, just tell Gemini what you want to add and ask for the exact steps and code.

## Step 5: Push Your Website to GitHub

Right now, your site only exists on your computer. GitHub stores your files online so Vercel can publish them.

1. Create a free GitHub account and click **New** to create a repository.
2. Give it a unique name and choose **Public** or **Private**.
3. Click **Create repository**.
4. Open a command prompt in your project folder. On Windows, click the folder's address bar, type `cmd`, and press Enter.
5. Run the commands GitHub shows you, followed by these to upload your files:

```bash
git init
git add .
git commit -m "Initial website upload"
git branch -M main
git remote add origin YOUR_REPOSITORY_URL
git push -u origin main
```

Replace `YOUR_REPOSITORY_URL` with the link GitHub gives you. Here's what each command does:

- `git add .` stages all the changes in your folder.
- `git commit -m` saves a snapshot with a short note describing the change.
- `git push` uploads that snapshot to GitHub.

Refresh your repository page, and you should see `index.html`, `style.css`, and `script.js`.

> **Pro Tip:** If you hit an error, copy the full error message and paste it into Gemini. It will usually tell you exactly how to fix it.

## Step 6: Deploy Your Website on Vercel

Now you'll make the site public.

1. Create a Vercel account and choose **Continue with GitHub**.
2. Click **New > Project**.
3. Find your repository and click **Import**.
4. Leave the default settings, as a simple HTML/CSS/JS site needs no special configuration.
5. Click **Deploy**.

After a short wait, you'll see a success message and a live subdomain. Open it, and your website is on the internet. Because Vercel is connected to GitHub, every time you push new changes, your site updates automatically.

## Step 7: Connect Your Own Domain

A subdomain works for testing, but a custom domain looks far more professional for a business or brand.

1. Buy a domain from a registrar such as [GoDaddy](AFFILIATE_LINK: https://www.godaddy.com).
2. In Vercel, go to **Domains**, click **Add Existing**, and enter your domain.
3. Vercel will show the DNS records you need to add.
4. In your registrar's DNS settings, add an **A record** with the name `@` and the IP address Vercel shows you.
5. Add a **CNAME record** with the name `www` and the value Vercel gives you.
6. Save both records and wait for DNS to propagate. This can take anywhere from a few minutes to several hours.

> **Pro Tip:** Always copy the exact values from your own Vercel dashboard. The IP and CNAME values can differ from the ones shown in tutorials.

## Ideas for What to Do Next

Once your site is live, you can keep improving it with AI:

- Ask Gemini to add new sections, pages, or a blog.
- Update your content and push changes to GitHub to redeploy instantly.
- Offer website building as a service, since this workflow lets you deliver sites fast.
- Use your site as the base for email outreach. When you're ready to send campaigns at scale, [InboxJet](https://www.smartivatetech.com/products/inboxjet) handles bulk sending with SMTP and API rotation.

## Conclusion

You've seen how to build and launch a real website without writing code yourself. Gemini writes the code, VS Code holds your files, GitHub stores them, and Vercel puts them online. The key is a clear prompt, reading each step, and asking the AI for complete code when you need it.

Stop just watching and start building. If you want to speed up this process and automate your workflows, check out the premium tools at [Smartivate](https://www.smartivatetech.com).