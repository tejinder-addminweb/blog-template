# Project Architecture

This document explains the structure and components of this Hugo site.

## 📁 Directory Structure

```
hugo-template/
├── archetypes/          # Content templates for hugo new
├── content/             # All content (Markdown files)
│   ├── _index.md       # Homepage content
│   ├── about.md        # About page
│   ├── archives.md     # Archives page
│   └── posts/          # Blog posts directory
│       ├── _index.md  # Posts list page
│       ├── example-post.md
│       └── first-post.md
├── layouts/            # HTML templates (custom theme)
│   ├── _default/       # Default page layouts
│   │   ├── baseof.html    # Base template
│   │   ├── index.html     # Homepage layout
│   │   ├── list.html      # List pages
│   │   ├── single.html    # Single post/page
│   │   ├── archives.html  # Archives page
│   │   ├── taxonomy.html # Tags/categories
│   │   └── terms.html     # Terms listing
│   └── partials/       # Reusable components
│       ├── head.html              # <head> content
│       ├── header.html            # Site header
│       ├── footer.html            # Site footer
│       ├── breadcrumbs.html       # Navigation breadcrumbs
│       ├── pagination.html        # Page pagination
│       ├── post-entry.html        # Post preview card
│       ├── post_meta.html         # Post metadata
│       ├── post-meta-date.html    # Date/time info
│       ├── post-meta-author.html  # Author info
│       ├── post_nav_links.html    # Previous/Next post
│       ├── share_icons.html       # Social sharing
│       └── social_icons.html      # Social links
├── static/             # Static assets
│   ├── css/
│   │   └── main.css    # All styles
│   └── js/
│       └── main.js     # All JavaScript
├── config.toml         # Site configuration
├── .gitignore          # Git ignore rules
├── README.md           # Main documentation
├── FEATURES.md         # Feature list
└── ARCHITECTURE.md     # This file
```

## 🎨 Theme Components

### No External Theme
This site uses **zero external theme dependencies**. All templates and styles are custom-built and self-contained.

### Layouts (_default/)

#### `baseof.html`
The foundation template that all pages extend. Contains:
- HTML document structure
- Head partial (meta tags, styles)
- Header partial (navigation)
- Main content area
- Footer partial
- JavaScript includes

#### `index.html`
Homepage layout:
- Welcome section with site title and description
- Recent posts listing
- Pagination for multiple pages

#### `list.html`
List page layout for:
- Posts listing
- Tags pages
- Categories pages
- Archive pages
- Displays breadcrumbs and post cards

#### `single.html`
Single post/page layout:
- Full post content
- Table of contents
- Post metadata
- Navigation links
- Share buttons

#### `archives.html`
Archives page layout:
- Groups posts by year
- Chronological listing
- Archive date format

#### `taxonomy.html`
Tags/Categories layout:
- Lists all posts in a tag/category
- Post cards with metadata

#### `terms.html`
Terms listing layout:
- Lists all tags/categories
- Shows post count per term

### Partials (reusable components)

#### Navigation
- **header.html**: Site header with logo and menu
- **breadcrumbs.html**: Location breadcrumb trail

#### Content
- **post-entry.html**: Post preview card
- **post_meta.html**: Post metadata wrapper
- **post-meta-date.html**: Date, reading time, word count
- **post-meta-author.html**: Author information

#### Navigation
- **post_nav_links.html**: Previous/Next post links
- **pagination.html**: Page number navigation

#### Social
- **share_icons.html**: Social sharing buttons
- **social_icons.html**: Social media links

#### Structure
- **head.html**: Meta tags, SEO, Open Graph
- **footer.html**: Site footer with copyright

## 🎨 Styling (CSS)

### File: `static/css/main.css`

**CSS Variables**: Theme colors defined as variables for easy customization

```css
:root {
    --bg: #fff;
    --text: #2d3748;
    --accent: #2563eb;
    /* ... */
}
```

**Dark Mode**: Full dark mode support via `[data-theme="dark"]`

**Responsive**: Mobile-first design with breakpoints at 768px

**Features**:
- Smooth transitions
- Hover effects
- Modern typography
- Code syntax highlighting
- Scroll animations
- Mobile menu
- Theme toggle button

## ⚙️ JavaScript (JS)

### File: `static/js/main.js`

**Features**:
- Mobile menu toggle
- Scroll to top button
- Smooth scrolling
- Code copy buttons
- Dark mode toggle
- Theme persistence in localStorage
- System theme detection

## ⚙️ Configuration

### File: `config.toml`

**Site Settings**:
- Title, description, author
- Base URL
- Language code

**Theme Settings**:
- Feature toggles (TOC, reading time, etc.)
- Theme variant (auto/light/dark)
- Social media links
- Menu configuration

**Markup Settings**:
- Goldmark extensions
- Syntax highlighting style
- Code fence line numbers

## 📝 Content Structure

### Markdown Files

All content in `content/` directory is Markdown.

**Front Matter**: YAML front matter for metadata
```yaml
---
title: "My Post"
date: 2024-01-01
tags: ["tag1", "tag2"]
showToc: true
---
```

**Markdown Features**:
- Headers (# ## ###)
- Bold (**text**), italic (*text*)
- Lists (- and 1.)
- Links and images
- Code blocks (```language)
- Tables
- Blockquotes (>)
- Emojis 🎉

## 🚀 Build Process

### Development
```bash
hugo server          # Start dev server
hugo server --watch  # Watch for changes
```

### Production
```bash
hugo                 # Build static site
```

Output goes to `public/` directory.

## 🎯 Key Features

### Self-Contained
- No npm dependencies
- No external themes
- No build tools required
- Pure Hugo + HTML/CSS/JS

### Performance
- Minimal JavaScript
- Optimized CSS
- Fast page loads
- Works offline

### SEO
- Meta tags
- Open Graph
- Twitter Cards
- Structured data
- Sitemap

### User Experience
- Dark mode
- Responsive design
- Smooth animations
- Mobile-friendly
- Accessible

## 🔧 Customization

### Colors
Edit CSS variables in `static/css/main.css`

### Features
Toggle features in `config.toml` under `[params]`

### Layouts
Modify templates in `layouts/`

### Content
Add/edit markdown files in `content/`

## 📚 Resources

- [Hugo Docs](https://gohugo.io/documentation/)
- [Markdown Guide](https://www.markdownguide.org/)
- [CSS Variables](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)

---

**Built with ❤️ using Hugo and custom templates**

