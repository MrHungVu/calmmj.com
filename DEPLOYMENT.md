# Deployment Guide for CalmMJ

## Current Status

The repository has a GitHub Actions workflow configured for automatic deployment to GitHub Pages.

## Setup Instructions

### Step 1: Enable GitHub Pages

1. Navigate to your repository on GitHub
2. Click on **Settings** (top right)
3. In the left sidebar, click on **Pages**
4. Under **Build and deployment**:
   - Source: Select **GitHub Actions**
   - Save the changes

### Step 2: Verify Workflow Permissions

The workflow already has the necessary permissions configured:
```yaml
permissions:
  contents: read
  pages: write
  id-token: write
```

### Step 3: Trigger Deployment

You can trigger deployment in two ways:

#### Option A: Push to Main Branch
```bash
git push origin main
```

#### Option B: Manual Workflow Dispatch
1. Go to the **Actions** tab in your repository
2. Click on **Deploy to GitHub Pages** workflow
3. Click **Run workflow** button
4. Select the `main` branch
5. Click **Run workflow**

## Expected Deployment URL

After successful deployment, your site will be available at:

**https://mrhungvu.github.io/calmmj.com/**

## Troubleshooting

### Deployment not working?

1. **Check GitHub Pages is enabled**:
   - Settings → Pages → Source should be "GitHub Actions"

2. **Check workflow runs**:
   - Go to Actions tab
   - Look for failed runs
   - Click on a run to see error details

3. **Verify permissions**:
   - The deploy workflow needs `pages: write` permission
   - This is already configured in the workflow file

4. **Check repository settings**:
   - Ensure the repository is public (or you have GitHub Pro for private repo pages)

### Common Issues

- **404 Error**: GitHub Pages not enabled in Settings
- **Permission denied**: Workflow permissions not properly configured
- **Build fails**: Check the Actions tab for error logs

## Workflow File Location

The deployment workflow is located at:
`.github/workflows/deploy.yml`

## Making Changes

To update the site:
1. Edit HTML files (index.html, about.html, services.html, contact.html)
2. Commit and push to main branch
3. Deployment happens automatically
4. Wait 1-2 minutes for changes to appear

## Support

For issues with GitHub Actions or deployment, check:
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)
