---
layout: default
title: Home
permalink: /
hero: true
subtitle: Welcome to Our Multi-Page Jekyll Site
---

## Quick Navigation

<div class="toc">
  <h3>Jump to Section</h3>
  <ul>
    <li><a href="#about-section">About This Site</a></li>
    <li><a href="#features-section">Features</a></li>
    <li><a href="#getting-started-section">Getting Started</a></li>
  </ul>
</div>

---

## About This Site {#about-section}

Welcome to our multi-page Jekyll website! This site demonstrates how to create a professional, multi-page site hosted on GitHub Pages with smooth scrolling anchor links and reusable components.

Each page is individually updatable and maintains a consistent design and navigation structure. The site uses Jekyll's powerful templating system to avoid repetition and make updates easy.

### Why Jekyll?

- **Simple**: No database required
- **Fast**: Generates static HTML
- **GitHub Pages**: Free hosting with automatic deployment
- **Version Control**: Track all changes with Git
- **Flexible**: Supports custom plugins and layouts

---

## Features {#features-section}

<div class="grid">
  <div class="card">
    <h4>🎨 Responsive Design</h4>
    <p>Works beautifully on desktop, tablet, and mobile devices with a fluid grid layout.</p>
  </div>
  
  <div class="card">
    <h4>⚡ Smooth Scrolling</h4>
    <p>Anchor links smoothly scroll to their sections with proper offset for the sticky navigation.</p>
  </div>
  
  <div class="card">
    <h4>🔗 Shared Components</h4>
    <p>Header, footer, and navigation are shared across all pages using Jekyll includes.</p>
  </div>
  
  <div class="card">
    <h4>📱 Mobile Optimized</h4>
    <p>Touch-friendly navigation and optimized performance for all devices.</p>
  </div>
  
  <div class="card">
    <h4>🚀 Easy Deployment</h4>
    <p>Deploy directly to GitHub Pages with a simple push to your repository.</p>
  </div>
  
  <div class="card">
    <h4>🎯 SEO Ready</h4>
    <p>Built-in SEO optimization with proper meta tags and semantic HTML.</p>
  </div>
</div>

---

## Getting Started {#getting-started-section}

### To deploy this site to GitHub Pages:

1. **Create a GitHub repository** named `yourusername.github.io`
2. **Copy all files** from this project to your repository
3. **Update `_config.yml`** with your information
4. **Push to GitHub** - your site will be live at `https://yourusername.github.io`

### To customize:

- Edit the individual page files (`.md` files) to update content
- Modify `_includes/` files to change components like header or footer
- Update `assets/css/style.css` to change colors and styling
- Change `_config.yml` to update site title and metadata

### To run locally:

```bash
gem install bundler
bundle install
bundle exec jekyll serve
```

Then visit `http://localhost:4000` in your browser.

---

**Next Steps:** Check out the [About page]({{ '/about' | relative_url }}) to see how other pages are structured!
