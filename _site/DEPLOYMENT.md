# GitHub Pages Deployment Guide

This guide will walk you through deploying your Jekyll site to GitHub Pages in just a few minutes.

## Step 1: Create a GitHub Pages Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon in the top right → **New repository**
3. Name your repository: **`yourusername.github.io`**
   - Replace `yourusername` with your actual GitHub username
   - Example: `john-doe.github.io`
4. Make sure it's set to **Public**
5. Click **Create repository**

## Step 2: Initialize Git and Push Your Code

Open Terminal/Command Prompt in the `jeckylSite` folder and run:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit with message
git commit -m "Initial Jekyll site"

# Rename branch to main (if on older git)
git branch -M main

# Add remote repository (replace yourusername)
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git push -u origin main
```

## Step 3: Wait for Deployment

GitHub Pages will automatically build and deploy your site. This usually takes 1-3 minutes.

Visit: **`https://yourusername.github.io`** to see your live site!

## Step 4: Customize for Your Use

Before pushing, you should update:

1. **_config.yml** - Update these lines:
   ```yaml
   title: Your Site Title
   description: Your site description
   url: "https://yourusername.github.io"
   author: Your Name
   email: your.email@example.com
   social:
     twitter: yourtwitter
     github: yourusername
   ```

2. **Each page** (.md files) - Replace dummy content with your own

3. **assets/css/style.css** - Change colors:
   ```css
   #667eea  /* Primary color - change this */
   #764ba2  /* Secondary color - change this */
   ```

## Step 5: Making Updates

To update your site after deployment:

```bash
# Edit files locally
# ... make your changes ...

# Commit and push
git add .
git commit -m "Update: Description of changes"
git push
```

Your site will automatically rebuild within a few minutes!

## Troubleshooting

### Site not showing?
- Wait 5-10 minutes, then hard refresh (Cmd+Shift+R on Mac, Ctrl+Shift+F5 on Windows)
- Check repository Settings → Pages → Source is set to "main" branch

### Build errors?
- Check [GitHub Pages Build Log](https://github.com/yourusername/yourusername.github.io/settings/pages)
- Common issues:
  - YAML syntax error in `_config.yml` - check indentation
  - Missing `_` in folder names
  - Plugins not in `Gemfile`

### Custom domain?
- See [GitHub Pages Custom Domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## Testing Locally (Optional)

Before pushing to GitHub, test locally:

```bash
# Install dependencies
bundle install

# Start development server
bundle exec jekyll serve

# Visit http://localhost:4000
```

Press `Ctrl+C` to stop the server.

---

**All set!** Your site is now live on GitHub Pages! 🎉
