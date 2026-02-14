# codebar's Organiser Hub

Documentation site for codebar organisers

## Prerequisites

- [Hugo](https://gohugo.io/) (extended version recommended)
- Git

## Quick Start

```bash
# Clone the repository
git clone git@github.com:mroderick/codebar-hugo-manual.git
cd hugo-manual

# Start development server
hugo server
```

Visit http://localhost:1313 to preview the site.

## Contributing

### Adding or Editing Pages

1. Create or edit content in `content/<slug>/index.md`
2. Use the following frontmatter format:

```yaml
+++
title = "Page Title"
weight = 10
aliases = ["/old-url.html"]
+++

Your content here...
```

- **`title`**: Page title displayed in the browser tab and sidebar
- **`weight`**: Controls sidebar order (lower numbers appear first)
- **`aliases`**: Creates redirects from old URLs

### Adding Images

Place images in `static/images/` and reference them as `/images/filename.png`.

### Running Locally

```bash
hugo server
```

The site will be available at http://localhost:1313

### Building for Production

```bash
hugo
```

The built site will be in the `public/` directory. **Do not commit the `public/` folder.**

## Theme

The site uses the `codebar-simple` theme located in `themes/codebar-simple/`.

- Templates: `themes/codebar-simple/layouts/`
- Styles: `themes/codebar-simple/assets/css/main.css`

## License

MIT
