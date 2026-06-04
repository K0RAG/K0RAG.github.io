# K0RAG.github.io — Personal Website

Black + neon purple personal site. Built with Jekyll and GitHub Pages.

---

## Deployment Instructions

### Step 1 — Delete the old repo content (or create fresh)

Go to: `https://github.com/K0RAG/K0RAG.github.io`

Either:
- **Option A (fresh start):** Delete the repo and recreate it with the same name `K0RAG.github.io`
- **Option B (overwrite):** Clone the existing repo and replace all files

### Step 2 — Clone your repo locally

```bash
git clone https://github.com/K0RAG/K0RAG.github.io.git
cd K0RAG.github.io
```

### Step 3 — Copy all site files into it

Copy everything from this folder into `K0RAG.github.io/`:

```
_layouts/
_posts/
assets/
blog/
projects/
my-work/
index.html
_config.yml
Gemfile
.gitignore
```

### Step 4 — Add your photo (optional but recommended)

1. Put your photo in `assets/img/aditya.jpg`
2. Open `index.html`
3. Find the comment `<!-- PHOTO INSTRUCTION -->`
4. Uncomment the `<img>` line and delete the placeholder `<div>`

### Step 5 — Update your LinkedIn username in _config.yml

Open `_config.yml` and set:
```yaml
linkedin_username: your-actual-linkedin-username
```
(The URL will become: `https://www.linkedin.com/in/your-actual-linkedin-username`)

### Step 6 — Push to GitHub

```bash
git add .
git commit -m "New site: black neon purple redesign"
git push origin main
```

### Step 7 — Enable GitHub Pages

1. Go to your repo → Settings → Pages
2. Source: Deploy from a branch
3. Branch: `main` → `/ (root)`
4. Click Save

Your site will be live at `https://k0rag.github.io` in ~2 minutes.

---

## How to Write a Blog Post

1. Create a file in `_posts/` named: `YYYY-MM-DD-post-title.md`
   - Example: `_posts/2026-06-04-my-thoughts-on-ai.md`

2. Add this at the top of the file (called "front matter"):
```yaml
---
layout: post
title: "Your Post Title"
date: 2026-06-04 00:00:00 +0530
tags: [thinking, tech]
excerpt: "One-sentence summary shown on the blog list."
---
```

3. Write your post below in Markdown

4. Push to GitHub:
```bash
git add _posts/2026-06-04-my-thoughts-on-ai.md
git commit -m "New post: My Thoughts on AI"
git push
```

The post appears on `/blog/` automatically with the correct date.

---

## How to Add a Project

Open `projects/index.html` and find the comment `<!-- ADD NEW PROJECT BELOW -->`.
Copy the project card block, fill in your details, save, and push.

## How to Add a Repository

Open `my-work/index.html` and find the comment `<!-- ADD MORE REPOS BELOW -->`.
Copy the repo card block, fill in your details, save, and push.

---

## File Structure

```
K0RAG.github.io/
├── _layouts/
│   ├── default.html     # main layout (nav + footer)
│   └── post.html        # blog post layout
├── _posts/
│   ├── 2026-02-06-why-this-site.md
│   └── 2026-02-06-first-blog.md
├── assets/
│   ├── css/
│   │   └── main.css     # all styles
│   └── img/             # put your photo here
├── blog/
│   └── index.html       # blog listing page
├── projects/
│   └── index.html       # projects page
├── my-work/
│   └── index.html       # repos & work page
├── index.html           # homepage
├── _config.yml          # Jekyll configuration
├── Gemfile              # Ruby dependencies
└── .gitignore
```
