# codebar's Organiser Hub

## Overview
Hugo-based documentation site for codebar, migrated from Jekyll. Hosted on GitHub Pages.

## Commands

### Development
```bash
hugo server
```
Starts local server at http://localhost:1313

### Build
```bash
hugo
```
Builds to `public/` directory (do not commit)

## Content Structure

### Adding a New Page
1. Create folder: `content/<slug>/index.md`
2. Use frontmatter:
```yaml
+++
title = "Page Title"
weight = 10
aliases = ["/old-url.html"]
+++

Content here...
```

- `weight`: Controls sidebar sort order (lower = higher)
- `aliases`: Creates redirects from old URLs

### Sidebar
- Automatically lists all pages in `content/` (excluding theme content)
- Sorted by `weight` frontmatter
- Excludes pages containing "post-1", "post-2", "post-3" in path

### Images
- Place in `static/images/`
- Reference as `/images/filename.png`

## Theme
- Theme: `themes/codebar-simple`
- CSS: `themes/codebar-simple/assets/css/main.css`
- Templates: `themes/codebar-simple/layouts/`

## Redirects
- Use `aliases` in frontmatter to create redirects from old URLs
- Example: `aliases = ["/old-page.html"]` generates redirect page
