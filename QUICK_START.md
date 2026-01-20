# Quick Start Guide - Mis|Disinformation Initiative Website

## 🚀 Test the Website Locally

```bash
cd /Users/saurabh/Desktop/Saurabh/misdisinfo.github.io
docker compose up
```

Visit: **http://localhost:8080**

## ✏️ Add Your First Content

### 1. Add a News Post

Create: `_posts/2026-01-21-your-title.md`

```markdown
---
layout: post
title: Your Title
date: 2026-01-21 10:00:00
tags: research events
categories: announcements
---

Your content here...
```

### 2. Add a Research Project

Create: `_projects/2_project-name.md`

```markdown
---
layout: page
title: Project Name
description: Brief description
importance: 1
category: current
---

Project details...
```

### 3. Add Publications

Edit: `_bibliography/papers.bib`

```bibtex
@article{yourpaper2026,
  title={Your Paper Title},
  author={Author Names},
  journal={Journal Name},
  year={2026},
  selected={true}
}
```

## 📝 Update Contact Info

Edit `_data/socials.yml`:

```yaml
email: your-actual-email@uva.nl
twitter_username: your_handle
github_username: your_org
```

## 🎨 Add Organization Logo

1. Save logo as `assets/img/prof_pic.jpg` (or any name)
2. Update in `_pages/about.md` frontmatter:

```yaml
profile:
  image: your-logo.jpg
```

## 📤 Deploy to GitHub

```bash
git add .
git commit -m "Update website content"
git push origin main
```

Auto-deploys via GitHub Actions → Available at https://misdisinfo.github.io

## 📚 Full Documentation

- **Website Management**: [WEBSITE_SETUP_GUIDE.md](WEBSITE_SETUP_GUIDE.md)
- **All Changes Made**: [CUSTOMIZATION_SUMMARY.md](CUSTOMIZATION_SUMMARY.md)
- **Detailed Options**: [CUSTOMIZE.md](CUSTOMIZE.md)

## ✅ Current Status

**Configured & Ready:**

- ✅ Organization branding
- ✅ Mission-focused about page
- ✅ Projects, Publications, Education pages
- ✅ News & Events blog
- ✅ Contact page
- ✅ Cleaned sample content

**Next: Add Your Content!**

1. Update social media handles
2. Add organization logo
3. Create real projects
4. Add publications
5. Write news posts
6. Update educational programs info

---

Need help? Check the documentation files or the [al-folio docs](https://github.com/alshedivat/al-folio).
