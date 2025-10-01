# CalmMJ - Mindful Journey

A peaceful wellness website focused on meditation techniques, breathing exercises, and wellness tips.

## 🌐 Live Site

Visit the live site at: **https://mrhungvu.github.io/calmmj.com/**

## 📁 Site Structure

- `index.html` - Homepage with welcome message
- `about.html` - About us page
- `services.html` - Services offered
- `contact.html` - Contact information

## 🚀 Deployment

This site is automatically deployed to GitHub Pages using GitHub Actions.

### Deployment Setup

1. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Under "Build and deployment", select **GitHub Actions** as the source

2. **Automatic Deployment**:
   - Any push to the `main` branch triggers automatic deployment
   - The workflow file is located at `.github/workflows/deploy.yml`

3. **Manual Deployment**:
   - Go to Actions tab → "Deploy to GitHub Pages"
   - Click "Run workflow" to manually trigger deployment

### Deployment Workflow

The deployment workflow:
1. Checks out the repository
2. Sets up GitHub Pages
3. Uploads site files as an artifact
4. Deploys to GitHub Pages

## 🛠️ Development

This is a static HTML site with no build process required. Simply edit the HTML files and commit to deploy.

## 📝 License

All rights reserved.
