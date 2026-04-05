# 🖋️ My Jekyll Blog — Setup Guide

A minimal, dark editorial Jekyll blog hosted on GitHub Pages.

## ✅ Features
- 4 pages: Home, About, Blog/Journal, Contact
- Static home page with your info (no posts shown)
- Blog section with post cards + full post reading
- Weekly post system — just add a file, done
- SEO optimized (meta tags, sitemap, RSS feed)
- GitHub Actions auto-deploy
- Contact form via Formspree (free, no backend)
- Mobile responsive

---

## 🚀 Setup (Step by Step)

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and click **New Repository**
2. Name it: `yourusername.github.io` ← replace with your GitHub username
3. Set it to **Public**
4. Don't initialize with README (you'll push this code)

### Step 2: Upload This Code

```bash
# In your terminal, navigate to this folder, then:
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOURUSERNAME/YOURUSERNAME.github.io.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under "Source", select **GitHub Actions**
3. The site will deploy automatically on every push!

Your site will be live at: `https://YOURUSERNAME.github.io`

---

## ✏️ Customize Your Info

### Personal Details
Edit `_config.yml`:
```yaml
title: "Your Name"
tagline: "Your Tagline"
author:
  name: "Your Name"
  email: "your@email.com"
  location: "Your City, Country"
  twitter: "yourhandle"
  github: "yourusername"
```

### Home Page
Edit `index.html` — change the bio text, stats, and skills section.

### About Page
Edit `pages/about.html` — update your story, timeline, and facts.

### Contact Page
Edit `pages/contact.html`:
1. Update the email link and social links
2. Sign up at [formspree.io](https://formspree.io) (free)
3. Create a new form and copy your Form ID
4. Replace `YOUR_FORM_ID` in the form action URL

### Add Your Photo
Put your photo in `assets/images/avatar.jpg` then in `index.html` and `pages/about.html` replace:
```html
<span class="avatar-placeholder">YN</span>
```
with:
```html
<img src="/assets/images/avatar.jpg" alt="Your Name">
```

---

## 📝 How to Write a New Post

Just create a new file in `_posts/` with this naming format:

```
_posts/YYYY-MM-DD-your-post-title.md
```

**Example:** `_posts/2025-02-05-my-new-post.md`

Every post needs this header at the top:

```yaml
---
layout: post
title: "Your Post Title Here"
date: 2025-02-05
category: Personal Growth
description: "A one-line summary of your post for SEO and previews."
emoji: "🌿"
read_time: 5
---

Your post content goes here...
```

That's it! Push to GitHub and your post is live. ✅

### Available Categories
Use any category you like. Some ideas:
- `Personal Growth`
- `Technology`
- `Books & Ideas`
- `Culture`
- `Life`

---

## 🏗️ File Structure

```
├── _config.yml          ← Site settings
├── _layouts/
│   ├── default.html     ← Main layout (nav + footer)
│   ├── post.html        ← Individual post layout
│   └── page.html        ← Static page layout
├── _posts/              ← YOUR BLOG POSTS GO HERE
│   └── YYYY-MM-DD-title.md
├── assets/
│   ├── css/main.scss    ← All styles
│   └── images/          ← Your images
├── pages/
│   ├── about.html
│   ├── blog.html
│   └── contact.html
├── index.html           ← Home page
├── Gemfile
└── .github/workflows/deploy.yml ← Auto-deploy
```

---

## 🛠️ Run Locally (Optional)

```bash
# Install Ruby first, then:
gem install bundler
bundle install
bundle exec jekyll serve

# Open: http://localhost:4000
```

---

## 🔍 SEO Notes

- Each page has proper `<title>` and meta description
- Open Graph tags for social sharing
- Sitemap auto-generated at `/sitemap.xml`
- RSS feed at `/feed.xml`
- Canonical URLs set correctly
- Post URLs follow `/blog/YYYY/MM/DD/title/` format for backlink preservation

---

## 📨 Questions?

If something doesn't work, check:
1. Repository is set to **Public**
2. GitHub Pages source is set to **GitHub Actions**
3. `_config.yml` has the correct `url` field
