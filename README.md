# Hugo Blog with PaperMod Theme

A complete Hugo static site with **PaperMod** theme - perfect for SEO-optimized blogging.

## Why PaperMod?

- 🔍 **SEO Optimized** - Built-in Open Graph tags, structured data, and meta tags
- ⚡ **Blazingly Fast** - Minimal JavaScript, optimized for performance
- 📱 **Mobile Responsive** - Perfect on all devices
- 🌙 **Dark Mode** - Automatic theme switching
- 📊 **Reading Stats** - Built-in reading time and word count
- 🎨 **Beautiful Design** - Clean, modern interface

## Getting Started

### Prerequisites

Make sure you have Hugo installed (Extended version recommended). Download from [gohugo.io](https://gohugo.io/getting-started/installing/).

### Initial Setup

1. Clone or download this project
2. Install the theme:

```bash
git submodule update --init --recursive
```

If you don't have the theme yet, run:
```bash
git submodule add -b master https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

### Running the Site

To start the Hugo development server, run:

```bash
hugo server
```

This will start a local development server at `http://localhost:1313`

### Building the Site

To build the static site for production:

```bash
hugo
```

The generated files will be in the `public/` directory.

## Project Structure

```
.
├── config.toml          # Hugo configuration file
├── content/             # Content files (Markdown)
│   ├── _index.md       # Homepage content
│   └── posts/          # Blog posts
├── layouts/            # HTML templates
│   ├── _default/       # Default templates
│   └── index.html      # Homepage template
├── archetypes/         # Content templates
└── public/             # Generated site (created after build)
```

## Creating New Content

### Create a New Post

```bash
hugo new posts/my-new-post.md
```

This will create a new post in the `content/posts/` directory with the proper front matter.

### Writing Content

All content is written in Markdown. PaperMod supports:

- ✅ Headers, bold, italic
- ✅ Images and links
- ✅ Lists and tables
- ✅ Code blocks with syntax highlighting
- ✅ Emoji support 🎉
- ✅ Table of Contents (auto-generated)

### Post Front Matter

Use these fields for better SEO:

```yaml
---
title: "Your Post Title"
date: 2024-01-01T10:00:00Z
draft: false
description: "A brief description for SEO"
tags: ["tag1", "tag2"]
showToc: true
tocOpen: false
---
```

## Customization

### Site Configuration

Edit `config.toml` to customize:
- Site title, description, and author
- Base URL
- Menu items
- Theme parameters

### SEO Settings

PaperMod includes built-in SEO features:
- Open Graph tags
- Twitter Cards
- Structured data (JSON-LD)
- Meta descriptions
- Canonical URLs

### Adding Features

PaperMod supports many extensions:
- Comments (Disqus, Utterances, etc.)
- Analytics (Google Analytics, Plausible)
- Social links
- Math rendering (KaTeX)
- Diagram support (Mermaid)

Check the [PaperMod documentation](https://github.com/adityatelange/hugo-PaperMod/wiki) for more options.

## Features

- Modern, responsive design
- Navigation menu
- Blog post listing
- Post metadata (date, author)
- SEO-friendly HTML structure
- Fast and lightweight

## Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [PaperMod Theme](https://github.com/adityatelange/hugo-PaperMod)
- [PaperMod Wiki](https://github.com/adityatelange/hugo-PaperMod/wiki)
- [Markdown Guide](https://www.markdownguide.org/)

## License

This is a template project. Modify it as needed for your use.

