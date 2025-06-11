# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll site for SaiJaiAI using the Chirpy theme. The site serves as a corporate website for an AI solutions competition platform. It features a custom landing page (`index.html`) with full SaiJaiAI branding while maintaining Jekyll's blog capabilities through the Chirpy theme structure.

## Development Commands

```bash
# Install dependencies
bundle install

# Serve locally for development (auto-reload enabled)
bundle exec jekyll serve

# Build for production
bundle exec jekyll build

# Test built site with HTMLProofer
bundle exec htmlproofer _site
```

Local development server runs at `http://localhost:4000`

## Architecture

**Jekyll + Chirpy Theme Structure:**
- Custom landing page in `index.html` (overrides theme default)
- Blog functionality available through `_posts/` directory
- Navigation tabs in `_tabs/` directory (about, archives, categories, tags)
- Site data configuration in `_data/` directory
- Theme assets and configurations inherited from jekyll-theme-chirpy

**Key Configuration:**
- `_config.yml`: Main Jekyll configuration (contains theme settings)
- `_data/contact.yml`: Contact options for the site
- `_data/share.yml`: Social sharing configuration
- Custom plugin in `_plugins/posts-lastmod-hook.rb` for Git-based post timestamps

## Important Notes

**Site Status:**
- Landing page is fully implemented and production-ready
- Jekyll blog features are configured but `_config.yml` contains placeholder values
- Theme supports PWA, analytics, comments, and SEO features

**Deployment:**
- Configured for GitHub Pages deployment
- Custom domain: `www.saijaiai.com` (via CNAME file)
- Automatic deployment on main branch push

**Content Management:**
- Add blog posts to `_posts/` directory using Jekyll naming convention
- Navigation pages are in `_tabs/` directory
- Static assets go in `assets/` directory
- Contact and social sharing options configured via `_data/` files

## Development Tips

- The site uses Jekyll's built-in SCSS processing
- Theme includes dark/light mode toggle functionality
- HTML/CSS compression is enabled for production builds
- Git-based last modified dates are automatically tracked for posts