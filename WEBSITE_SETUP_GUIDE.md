# Mis|Disinformation Initiative Website - Setup Guide

This document provides instructions for managing and updating the Mis|Disinformation Initiative website.

## Website Structure

The website has been configured with the following sections:

### Main Pages

1. **About** (`/`) - Homepage with initiative mission and goals
2. **Projects** (`/projects/`) - Research projects (current and completed)
3. **Publications** (`/publications/`) - Academic publications and research outputs
4. **Education** (`/education/`) - Educational programs and training opportunities
5. **News & Events** (`/blog/`) - Latest updates, announcements, and events
6. **Contact** (`/contact/`) - Contact information and inquiry form

### Disabled Pages

The following pages are disabled (not shown in navigation) but can be re-enabled if needed:
- CV page
- Books/bookshelf page
- Individual profiles page

## Adding Content

### Adding News & Blog Posts

Create a new file in `_posts/` with the naming format: `YYYY-MM-DD-title.md`

Example:
```markdown
---
layout: post
title: Your Post Title
date: 2026-01-20 10:00:00
description: Brief description
tags: research events
categories: announcements
---

Your content here...
```

### Adding Projects

Create a new file in `_projects/` with the naming format: `number_project-name.md`

Example:
```markdown
---
layout: page
title: Project Title
description: Brief description
img: assets/img/project-image.jpg
importance: 1
category: current # or 'completed'
---

Project details here...
```

### Adding Publications

Add publications to `_bibliography/papers.bib` in BibTeX format. Mark important publications with `selected={true}`.

### Adding News Announcements

Create short announcements in `_news/` for the homepage news section:

```markdown
---
layout: post
title: Short Announcement
date: 2026-01-20
inline: true
---

Brief announcement text here.
```

## Configuration

### Site Settings

Edit `_config.yml` to modify:
- Site title and description
- Contact information
- Enabled features
- Theme colors
- Blog settings

### Social Media & Contact

Edit `_data/socials.yml` to update:
- Email address
- Social media handles
- Custom links

### Navigation Menu

Edit page frontmatter to control navigation:
- `nav: true` - Show in navigation
- `nav: false` - Hide from navigation
- `nav_order: 3` - Position in menu

## Testing Locally

### Using Docker (Recommended)

```bash
docker compose up
```

Visit: http://localhost:8080

### Using Jekyll Directly

```bash
bundle install
bundle exec jekyll serve
```

Visit: http://localhost:4000

## Deployment

The site automatically deploys to GitHub Pages when you push to the `main` branch.

## Content Guidelines

### Writing Style
- Use clear, accessible language
- Avoid excessive jargon
- Write for diverse audiences (researchers, students, public)

### Images
- Place images in `assets/img/`
- Use descriptive filenames
- Optimize file sizes for web

### Links
- Use relative links for internal pages: `/projects/`
- Use absolute URLs for external sites
- Check links regularly for broken references

## Maintenance Tasks

### Regular Updates
- Add new publications as they're released
- Post news about events and activities
- Update project statuses
- Review and update educational program information

### Quarterly Reviews
- Check for broken links
- Update team member information
- Review analytics (if configured)
- Update event archives

## Support

For technical issues or questions about the website:
- Review the original [CUSTOMIZE.md](CUSTOMIZE.md) for detailed customization options
- Check [FAQ.md](FAQ.md) for common issues
- Consult the [al-folio documentation](https://github.com/alshedivat/al-folio)

## Key Features Configured

✅ Organization-focused design (not individual portfolio)
✅ Research projects showcase
✅ Publications with BibTeX integration
✅ Education programs page
✅ News & events blog
✅ Contact page
✅ Social media integration
✅ Responsive design
✅ Search functionality
✅ Dark mode support

## Next Steps

1. **Update social media information** in `_data/socials.yml` with actual handles
2. **Add team members** (consider re-enabling profiles page or creating a team section)
3. **Add real projects** by editing files in `_projects/`
4. **Add publications** to `_bibliography/papers.bib`
5. **Create news posts** about your activities and events
6. **Add organization logo** to `assets/img/` and update in pages
7. **Configure analytics** (optional) in `_config.yml`
8. **Set up custom domain** (optional) following GitHub Pages documentation

## Contact & Collaboration

This website serves as a hub for collaboration and knowledge sharing. Encourage visitors to:
- Subscribe to updates
- Follow on social media
- Reach out for collaborations
- Participate in events
- Share publications and insights
