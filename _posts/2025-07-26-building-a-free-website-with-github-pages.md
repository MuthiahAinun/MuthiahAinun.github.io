---
layout: post
title: "Building a Free Website with GitHub Pages"
author: Muthiah
categories: literature
---

<center>
  <img src="https://live.staticflickr.com/65535/54675040142_2672de0c37_n.jpg" alt="ML Journey" style="border-radius: 8px; margin-bottom: 1em;">
</center>

> Tired of seeing cool personal websites and wishing you had one too? The good news is you can have one, for free!
No ads. No limited features. And yes , you control everything, just using GitHub.
Even if you're a beginner, I'll walk you through it step-by-step.

#### 🚀 Why GitHub?

You may have tried free sites like WordPress, but they come with limitations , annoying ads, locked features, or themes you can't fully customize.

GitHub Pages gives you:

- 💸 100% free hosting

- 🧩 Full control over the code & theme

- 🛠️ No backend or complex setup

- 🌐 A real `yourname.github.io` domain

If you're into coding (or want to learn!), this is a fun and empowering way to build your own personal website.

#### 🛠️ What You'll Need (for Windows users)

Before building your site, install these tools:

| Tool                                                       | Purpose                         | Link                                                   |
|------------------------------------------------------------|----------------------------------|--------------------------------------------------------|
| Git                                                        | Version control & cloning repos | [Download Git](https://git-scm.com/downloads/win)      |
| VS Code                                                    | Code editor                     | [Visual Studio Code](https://code.visualstudio.com/)   |
| Ruby + Devkit                                              | For Jekyll theme engine         | [Ruby Installer](https://rubyinstaller.org/downloads/) |
| PowerShell                                                 | Terminal interface              | Pre-installed, or update via command below             |


> ✅ After installing Ruby, select to install `ridk`. In the terminal, type `3` and hit Enter.

> `winget install --id Microsoft.Powershell --source winget` for PowerShell *(Run in CMD as Administrator)*

#### 📦 Step-by-Step Guide

1.**Create Your GitHub Account and Repository**

- Go to GitHub and sign up.
- Click the ➕ icon (top right) → **New Repository**
- Name your repo using this format: `YourUsername.github.io`, e.g. `MuthiahAinun.github.io`.
- Check Add `README.md` → Click **Create repository**

2.**Find a Jekyll Theme**

- Go to [Jekyll Themes](jekyllthemes.io/free), Choose a free theme you like and click **Get *themename* on Github**.
- Copy the link. For example:
Theme link: https://github.com/niklasbuschmann/contrast

3.**Open PowerShell and Clone the Theme**

```
git clone https://github.com/niklasbuschmann/contrast.git

```
Then **create a new folder** with your GitHub repo name:
```
mkdir MuthiahAinun.github.io

```

**Move** the theme files:
```
mv contrast MuthiahAinun.github.io/
cd MuthiahAinun.github.io

```
4.**Activate Jekyll**

Install required gems:
```
gem install jekyll bundler
jekyll -v
bundle install

```

5.**Open the Project in VS Code**

```
code .

```
Edit these important files:

- `_config.yml` → Change site title, email, description

- `Gemfile` → Add any missing dependencies if needed

- `_data/menu.yml` → Customize navigation menu

Example to add a "Gallery" tab:

```
- title: Galeri
  url: /galeri.html

```
- `_posts` → Place your blog posts or content here

6.**Preview Your Website Locally**

To test before uploading to GitHub:

```
bundle exec jekyll serve
```

Visit `http://localhost:4000` in your browser to view it.

7.**Connect to Your GitHub Repo**

Clone your own GitHub repo:

For Example:
```
git clone https://github.com/MuthiahAinun/MuthiahAinun.github.io.git
```
Copy your final website files into this repo folder.

Push your code to GitHub:
```
git add .
git commit -m "Upload website"
git push origin main
```
#### ✅ Done! Your Website Is Live

Open your browser and visit it.
For Example:
🔗 `https://MuthiahAinun.github.io`
Your personal website is now live and accessible to the world!

#### 📝 Final Tips
- You can always change the theme later : just follow the same process.
- You can connect a custom domain if you want (e.g. with Freenom).
- This is great for portfolios, blogs, resume sites, or even project documentation.

> 💬 "You don’t have to wait to be an expert to build something online. Start messy, and grow along the way." 