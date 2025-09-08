# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static personal portfolio website for Michael Raffelsberger, deployed via GitHub Pages. The site showcases professional experience, skills, and projects in data science and AI.

## Architecture

### File Structure
- `index.html` - Main HTML file with complete site structure, SEO metadata, and structured data
- `styles.css` - Complete CSS with CSS custom properties for theming, responsive design, and animations  
- `main.js` - JavaScript for interactive features (stars animation, theme toggle, smooth scrolling)
- `images/` - Static assets including profile photo
- `sitemap.xml` - SEO sitemap
- `robots.txt` - Search engine directives
- `googlef5f82385e4e4a5dd.html` - Google Search Console verification

### Design System
- **Theming**: CSS custom properties with dark/light theme support via `data-theme` attribute
- **Responsive**: Mobile-first approach with CSS Grid and Flexbox
- **Animations**: CSS animations for stars background, hover effects, and theme transitions
- **Typography**: Inter font family with semantic color tokens

### Key Features
- **Theme Toggle**: JavaScript-powered dark/light mode with localStorage persistence
- **Animated Background**: Procedurally generated twinkling stars
- **Smooth Scrolling**: Navigation with smooth scroll behavior
- **Timeline Component**: Professional experience displayed in alternating timeline format
- **Skills Grid**: Categorized technical skills with tags
- **SEO Optimized**: Complete meta tags, structured data (JSON-LD), Open Graph, and Twitter cards

## Development

### No Build Process
This is a static site with no build tools, package.json, or dependencies. Changes can be made directly to HTML, CSS, and JavaScript files.

### Local Development
Serve files with any static server:
```bash
python -m http.server 8000
# or
npx serve .
```

### Deployment
Site auto-deploys to GitHub Pages on push to main branch via standard GitHub Pages hosting.

## GitHub Integration

The repository includes Claude Code GitHub Action configuration (`.github/workflows/claude.yml`) for automated assistance triggered by `@claude` mentions in issues and pull requests.