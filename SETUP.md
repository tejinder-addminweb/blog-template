# Quick Setup Guide

## Step 1: Install the PaperMod Theme

Run this command to add the theme as a submodule:

```bash
git submodule add -b master https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

Or if you're cloning this project fresh:

```bash
git submodule update --init --recursive
```

## Step 2: Start the Server

```bash
hugo server -D
```

The `-D` flag includes draft posts. Remove it once your posts are ready.

## Step 3: View Your Site

Open your browser to: `http://localhost:1313`

## What's Been Configured?

✅ **PaperMod Theme** - SEO-optimized blogging theme  
✅ **Homepage** - Welcome page with site info  
✅ **Blog Posts** - Sample posts to get you started  
✅ **About Page** - Personal introduction page  
✅ **Archives** - All posts listing  
✅ **Search** - Site search functionality  
✅ **Menu Navigation** - Easy site navigation  
✅ **SEO Settings** - Meta tags, descriptions, Open Graph  
✅ **Reading Time** - Auto-calculated reading stats  
✅ **Table of Contents** - Auto-generated TOC for posts  
✅ **Dark Mode** - Automatic theme switching  

## Next Steps

1. Edit `config.toml` to customize your site details
2. Create new posts with: `hugo new posts/your-post-title.md`
3. Customize the theme in `config.toml`
4. Add images to the `static/` folder
5. Configure analytics and comments (check PaperMod docs)

## PaperMod Features for SEO

This theme includes:
- Open Graph tags for social sharing
- Twitter Card support
- Structured data (JSON-LD)
- Meta descriptions
- Canonical URLs
- Sitemap generation
- RSS feed
- Reading time and word count

## Learn More

- [PaperMod Documentation](https://github.com/adityatelange/hugo-PaperMod/wiki)
- [PaperMod Examples](https://adityatelange.github.io/hugo-PaperMod/)
- [Hugo Quick Start](https://gohugo.io/getting-started/quick-start/)

