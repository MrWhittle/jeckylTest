# Multi-Page Jekyll Site with Anchored Links

A professional, responsive Jekyll site hosted on GitHub Pages featuring smooth-scrolling anchor links, shared components, and easily updatable content across 5 pages.

## Features

- ✅ **5 Easy-to-Update Pages**: Home, About, Services, Portfolio, Contact
- ✅ **Anchored Links**: Smooth-scrolling navigation between sections on each page
- ✅ **Shared Components**: Reusable header, footer, and navigation
- ✅ **Responsive Design**: Works perfectly on desktop, tablet, and mobile
- ✅ **GitHub Pages Ready**: Deploy directly with no extra setup
- ✅ **Customizable styling**: Easy-to-modify CSS
- ✅ **SEO Optimized**: Meta tags and semantic HTML included
- ✅ **Back-to-Top Button**: Smooth scroll back to top with auto-show

## Quick Start

### Prerequisites

- Ruby 2.7 or higher
- Bundler (install with `gem install bundler`)
- Git

### Local Setup

```bash
# Clone your repository
git clone https://github.com/yourusername/yourusername.github.io.git
cd yourusername.github.io

# Install dependencies
bundle install

# Start the development server
bundle exec jekyll serve

# Visit http://localhost:4000 in your browser
```

### Customization

1. **Site Title & Description**: Edit `_config.yml`
2. **Page Content**: Edit the `.md` files (index.md, about.md, services.md, portfolio.md, contact.md)
3. **Styling**: Modify `assets/css/style.css`
4. **Header/Footer/Navigation**: Edit files in `_includes/`
5. **Colors & Gradients**: Search for hex codes in `style.css` and `_includes/hero.html`

### Page Structure

Each page includes:
- A hero section (optional, controlled by `hero: true` in frontmatter)
- Table of contents with anchor links
- Multiple sections with IDs for anchored linking
- Dummy content ready to customize

#### Creating Anchor Links

Add a section ID like this:
```markdown
## Section Title {#section-id}

Content goes here...
```

Then link to it:
```markdown
[Link to Section]({{ '/page' | relative_url }}#section-id)
```

## Deployment to GitHub Pages

### Step 1: Create Repository

1. Go to GitHub and create a new repository named `yourusername.github.io`
2. Make sure it's set to Public

### Step 2: Push Code

```bash
git init
git add .
git commit -m "Initial Jekyll site"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

### Step 3: Enable GitHub Pages (if not automatic)

1. Go to repository Settings → Pages
2. Set Source to "Deploy from a branch"
3. Select `main` branch and `/root` folder
4. Save

Your site will be live at `https://yourusername.github.io` within minutes!

## File Structure

```
├── _config.yml           # Jekyll configuration
├── _layouts/
│   └── default.html      # Main page layout
├── _includes/
│   ├── header.html       # Site header
│   ├── footer.html       # Site footer
│   ├── navigation.html   # Navigation menu
│   └── hero.html         # Hero section template
├── assets/
│   ├── css/
│   │   └── style.css     # Main stylesheet
│   └── js/
│       └── script.js     # Client-side JavaScript
├── index.md              # Home page
├── about.md              # About page
├── services.md           # Services page
├── portfolio.md          # Portfolio page
├── contact.md            # Contact page
├── Gemfile               # Ruby dependencies
└── README.md             # This file
```

## Adding a Contact Form

Since this is a static site, you have several options:

### Option 1: Formspree (Recommended)
1. Go to [formspree.io](https://formspree.io)
2. Create a new form and get your form ID
3. Create an HTML contact form that posts to Formspree

### Option 2: Netlify Forms
Deploy to Netlify instead of GitHub Pages and use built-in form handling

### Option 3: Basin
Use [basin.io](https://basin.io) for simple form backend

## Customizing Colors

Edit `assets/css/style.css` to change the color scheme:

```css
/* Primary gradient color (currently purple/blue) */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

Change `#667eea` and `#764ba2` to your preferred colors.

## Adding More Pages

1. Create a new `.md` file in the root directory
2. Add frontmatter:
   ```yaml
   ---
   layout: default
   title: Page Title
   permalink: /page-name
   hero: true
   ---
   ```
3. Add content with sections that have IDs for anchoring
4. Update navigation in `_includes/navigation.html`

## Tips for Success

- Use descriptive section IDs (e.g., `#pricing-section` not `#s1`)
- Keep content scannable with headers and bullet points
- Use the `.card` and `.grid` classes for content layouts
- Test on mobile using browser DevTools
- Keep images optimized for web
- Update author info in `_config.yml`

## Troubleshooting

**Site not building?**
- Check `_config.yml` for YAML syntax errors
- Ensure all file names start with underscore if in special directories
- Re-run `bundle install`

**Links not working?**
- Use the `relative_url` filter: `{{ '/page' | relative_url }}`
- Check permalink in page frontmatter
- Reload the browser cache (Cmd+Shift+R)

**Styles not applying?**
- Hard refresh browser (Cmd+Shift+R on Mac, Ctrl+Shift+F5 on Windows)
- Check that CSS file path is correct in layout
- Verify CSS file has .css extension

## Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Docs](https://docs.github.com/en/pages)
- [Markdown Syntax](https://guides.github.com/features/mastering-markdown/)
- [YAML Frontmatter](https://jekyllrb.com/docs/front-matter/)

## License

This project is open source and available under the MIT License.

## Support

For questions or issues:
1. Check the [Jekyll docs](https://jekyllrb.com/docs/)
2. Visit [GitHub Pages help](https://docs.github.com/en/pages)
3. Create an issue in your repository

---

**Happy building!** 🚀 Deploy this site to GitHub Pages and start customizing it for your needs.
