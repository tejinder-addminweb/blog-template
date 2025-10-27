# Modern Hugo Blog - No Theme Required!

A complete, self-contained Hugo static site with beautiful modern design - no external theme dependencies!

## ✨ Features

- 🌙 **Dark Mode** - Automatic theme detection with manual toggle
- 📱 **Responsive Design** - Perfect on all devices
- 🔍 **SEO Optimized** - Meta tags, Open Graph, Twitter Cards
- ⚡ **Blazing Fast** - Minimal JavaScript, optimized CSS
- 📊 **Reading Stats** - Automatic reading time and word count
- 🔖 **Table of Contents** - Auto-generated for long articles
- 📝 **Code Highlighting** - Syntax highlighting with copy buttons
- 🌐 **Social Sharing** - Easy sharing to social media
- 📡 **RSS Feed** - Subscribe to get updates
- 🎨 **Beautiful UI** - Clean, modern design

## 🚀 Getting Started

### Prerequisites

Make sure you have Hugo installed (Extended version recommended). Download from [gohugo.io](https://gohugo.io/getting-started/installing/).

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd hugo-template
   ```

2. **Run the development server**
   ```bash
   hugo server
   ```

   Your site will be available at `http://localhost:1313`

3. **Build for production**
   ```bash
   hugo
   ```

   The generated files will be in the `public/` directory.

## 📁 Project Structure

```
.
├── config.toml          # Hugo configuration
├── content/             # Content files (Markdown)
│   ├── _index.md       # Homepage content
│   ├── about.md        # About page
│   ├── archives.md     # Archives page
│   └── posts/          # Blog posts
├── layouts/            # HTML templates
│   ├── _default/       # Default page templates
│   └── partials/       # Reusable components
├── static/             # Static assets
│   ├── css/            # Stylesheets
│   └── js/             # JavaScript files
└── public/             # Generated site (after build)
```

## ✍️ Creating Content

### Create a New Post

```bash
hugo new posts/my-new-post.md
```

This will create a new post in the `content/posts/` directory with proper front matter.

### Post Front Matter

Use these fields for better SEO and features:

```yaml
---
title: "Your Post Title"
date: 2024-01-01T10:00:00Z
draft: false
description: "A brief description for SEO"
tags: ["tag1", "tag2"]
categories: ["Category"]
author: "Author Name"
showToc: true
showShareButtons: true
---
```

## 🎨 Customization

### Site Configuration

Edit `config.toml` to customize:

- Site title, description, and author
- Base URL
- Menu items
- Theme parameters
- Social media links

### Theme Parameters

```toml
[params]
  # Feature toggles
  showToc = true              # Table of contents
  showReadingTime = true      # Reading time
  showWordCount = true        # Word count
  showBreadcrumbs = true      # Breadcrumb navigation
  disableThemeToggle = false  # Disable dark mode toggle
  disableScrollToTop = false  # Disable scroll to top button
  ShowCodeCopyButtons = true  # Code copy buttons
  
  # Theme
  themeVariant = "auto"       # auto, light, dark
```

### Social Links

Add your social media links in `config.toml`:

```toml
[params.socialIcons]
  email = "mailto:your@email.com"
  github = "https://github.com/yourusername"
  twitter = "https://twitter.com/yourusername"
  linkedin = "https://linkedin.com/in/yourusername"
```

## 🎯 SEO Features

This site includes:

- ✅ Open Graph tags for social media
- ✅ Twitter Cards
- ✅ Structured data (JSON-LD)
- ✅ Meta descriptions
- ✅ Canonical URLs
- ✅ Sitemap generation
- ✅ RSS feed

## 🚢 Deployment

### GitHub Pages

1. Build your site: `hugo`
2. Deploy the `public/` folder to GitHub Pages

### Netlify

1. Connect your repository to Netlify
2. Build command: `hugo`
3. Publish directory: `public`

### Vercel

1. Connect your repository to Vercel
2. Build command: `hugo`
3. Output directory: `public`

## 💡 Tips

### Writing Content

- Use Markdown for all content
- Add front matter to every page
- Use tags and categories for organization
- Include descriptions for SEO

### Performance

- Images are lazy-loaded by default
- CSS is optimized and minified
- JavaScript is minimal and efficient
- Fast page loads even on slow connections

### Development

- Watch for changes: `hugo server --watch`
- Build drafts: `hugo server -D`
- Check future dates: `hugo server --buildFuture`

## 🔧 Troubleshooting

### Theme not loading?

Make sure to run `hugo` without any theme in `config.toml`.

### Styles not appearing?

Check that your CSS files are in the `static/css/` directory.

### JavaScript not working?

Ensure JavaScript files are in `static/js/` and referenced correctly.

## 📚 Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [Markdown Guide](https://www.markdownguide.org/)
- [Static Site Generators](https://www.staticgen.com/)

## 📄 License

This is a template project. Modify it as needed for your use.

## 🙏 Credits

Built with:
- [Hugo](https://gohugo.io/) - Static site generator
- Custom CSS with modern design patterns
- Minimal JavaScript for optimal performance

---

**Ready to start blogging? Run `hugo server` and begin!** 🚀
