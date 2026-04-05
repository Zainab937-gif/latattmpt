# Dark Bold Jekyll Blog 🖤

Ek clean, dark-themed Jekyll blog — GitHub Pages ke liye bilkul ready.

## ⚡ 5 Minute Setup

### Step 1: Fork karo
Upar "Fork" button click karo.

### Step 2: Rename karo
Repo ka naam rakho: `TUMHARA-USERNAME.github.io`
(Settings > General > Repository name)

### Step 3: `_config.yml` update karo
```yaml
title: "./tumhara-blog"         # Apna naam
author: "Tumhara Naam"
url: "https://TUMHARA-USERNAME.github.io"
github_username: TUMHARA-USERNAME
```

### Step 4: GitHub Pages on karo
Settings > Pages > Source: **Deploy from a branch** > Branch: `main` > Save

### Step 5: Wait karo (2-3 min)
Phir jao: `https://TUMHARA-USERNAME.github.io` 🎉

---

## ✍️ Naya Post Likhna

`_posts/` folder mein file banao:

**Filename:** `YYYY-MM-DD-title.md`  
Example: `2024-04-05-mera-pehla-post.md`

**Top mein ye likho (Front Matter):**
```yaml
---
layout: post
title: "Post ka Title"
date: 2024-04-05
tags: [tag1, tag2]
excerpt: "Chhoti si summary jo homepage pe dikhegi."
---

Yahaan apna content likho...
```

---

## 📁 Folder Structure

```
.
├── _config.yml          ← Blog settings (ZAROOR edit karo)
├── _layouts/            ← Page templates
├── _includes/           ← Header, Footer
├── _posts/              ← Tumhare blog posts (yahaan likho)
├── assets/css/main.css  ← Saara styling
├── index.html           ← Homepage
├── about.html           ← About page
├── archive.html         ← Saare posts
└── tags.html            ← Tags se browse karo
```

---

## 🎨 Customization

**Font change karna:** `assets/css/main.css` mein `@import` URL update karo.

**Accent color change karna:** `main.css` mein `--accent: #f5e642;` update karo.

**Naya page banana:**
```yaml
---
layout: default
title: "Page Title"
permalink: /page-url/
---
Content yahaan...
```
