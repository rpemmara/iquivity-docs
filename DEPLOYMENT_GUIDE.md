# GitHub Pages Deployment Guide

Complete guide to deploying iQuivity documentation to GitHub Pages.

## 📋 Prerequisites

Before you begin, ensure you have:
- Git installed on your computer
- A GitHub account
- Repository access (or create a new repository)

## 🚀 Step-by-Step Deployment

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com)
2. Click the **"+"** icon → **"New repository"**
3. Repository settings:
   - **Name**: `iquivity-docs` (or your preferred name)
   - **Description**: "iQuivity Platform Documentation"
   - **Visibility**: Public (required for free GitHub Pages)
   - **DO NOT** initialize with README, .gitignore, or license
4. Click **"Create repository"**

### Step 2: Configure Repository URL

1. Open `mkdocs.yml` in your text editor
2. Find line 4:
   ```yaml
   site_url: https://[your-github-username].github.io/[your-repo-name]/
   ```
3. Replace with your actual values:
   ```yaml
   site_url: https://your-username.github.io/iquivity-docs/
   ```
   Example: `site_url: https://johndoe.github.io/iquivity-docs/`

### Step 3: Initialize and Push Repository

Open terminal/command prompt in the project directory and run:

```bash
# If not already initialized (check with 'git status')
git init

# Change default branch to 'main' (if needed)
git branch -M main

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: iQuivity documentation"

# Add your GitHub repository as remote
# Replace with your repository URL
git remote add origin https://github.com/your-username/iquivity-docs.git

# Push to GitHub
git push -u origin main
```

**Important**: Replace `your-username` and `iquivity-docs` with your actual GitHub username and repository name.

### Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Build and deployment"**:
   - **Source**: Select "GitHub Actions" (recommended)
   - This allows the workflow to deploy automatically
5. Click **"Save"** if needed

### Step 5: Wait for Deployment

1. Go to the **"Actions"** tab in your repository
2. You should see a workflow running: "Deploy Documentation"
3. Wait for it to complete (usually 1-3 minutes)
4. Green checkmark ✓ means successful deployment

### Step 6: Access Your Documentation

Once deployed, your documentation will be available at:
```
https://your-username.github.io/iquivity-docs/
```

Example: `https://johndoe.github.io/iquivity-docs/`

## 🔧 Configuration Details

### GitHub Actions Workflow

The deployment is automated via `.github/workflows/deploy-docs.yml`:

```yaml
name: Deploy Documentation

on:
  push:
    branches:
      - main
      - master
  workflow_dispatch:

permissions:
  contents: write

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Set up Python
        uses: actions/setup-python@v4
      - name: Install MkDocs
        run: |
          pip install mkdocs-material
          pip install mkdocs-awesome-pages-plugin
      - name: Deploy
        run: mkdocs gh-deploy --force
```

**What it does:**
- Triggers on push to `main` or `master` branch
- Sets up Python environment
- Installs MkDocs and dependencies
- Builds and deploys to `gh-pages` branch

### Repository Structure

```
your-repository/
├── .github/
│   └── workflows/
│       └── deploy-docs.yml       # Auto-deployment workflow
├── docs/                         # Documentation source files
│   ├── index.md
│   ├── getting-started/
│   ├── features/
│   ├── chatbots/
│   ├── marketing/
│   └── account/
├── .gitignore                    # Git ignore file
├── mkdocs.yml                    # MkDocs configuration
├── requirements.txt              # Python dependencies
├── DOCS_README.md               # Documentation README
└── DEPLOYMENT_GUIDE.md          # This file
```

## 🔄 Making Updates

### Update Documentation

1. Edit files in the `docs/` directory
2. Test locally (optional):
   ```bash
   mkdocs serve
   # Visit http://127.0.0.1:8000
   ```
3. Commit changes:
   ```bash
   git add .
   git commit -m "Update: [describe your changes]"
   git push
   ```
4. GitHub Actions will automatically rebuild and deploy

### Update Configuration

If you modify `mkdocs.yml`:
1. Make your changes
2. Commit and push
3. Automatic deployment will apply new configuration

## 🐛 Troubleshooting

### Workflow Fails

**Check the error logs:**
1. Go to "Actions" tab
2. Click on the failed workflow
3. Expand the failed step to see error details

**Common issues:**

1. **Missing dependencies**
   - Ensure `requirements.txt` includes all needed packages
   - Verify `mkdocs-material` and `mkdocs-awesome-pages-plugin` are listed

2. **Invalid markdown**
   - Check for syntax errors in `.md` files
   - Ensure all internal links are correct

3. **Permission denied**
   - Go to Settings → Actions → General
   - Under "Workflow permissions", select "Read and write permissions"

### Site Not Accessible

1. **Check Pages settings:**
   - Settings → Pages
   - Source should be "GitHub Actions"
   - Check for any error messages

2. **DNS propagation:**
   - Wait 5-10 minutes after first deployment
   - Clear browser cache

3. **404 errors:**
   - Verify `site_url` in `mkdocs.yml` matches your actual URL
   - Ensure it ends with `/`

### Local Preview Issues

If `mkdocs serve` doesn't work:

```bash
# Install/update dependencies
pip install --upgrade -r requirements.txt

# Or install individually
pip install mkdocs-material
pip install mkdocs-awesome-pages-plugin
```

## 📊 Monitoring Deployments

### View Deployment Status

**Actions Tab:**
- See all workflow runs
- View logs for debugging
- Re-run failed workflows

**Pages Tab:**
- Check current deployment status
- View deployment history
- See any deployment errors

### Build Time

Typical deployment times:
- First deployment: 2-4 minutes
- Subsequent deployments: 1-2 minutes

## 🔒 Security & Permissions

### Repository Visibility

**Public Repository (Free):**
- ✅ GitHub Pages works automatically
- ✅ Anyone can view documentation
- ✅ Anyone can view source

**Private Repository:**
- ❌ GitHub Pages requires GitHub Pro/Team/Enterprise
- Consider making docs repository public even if code is private

### Workflow Permissions

Required permissions for deployment:
- **Contents**: write (to push to gh-pages branch)

Set in: Settings → Actions → General → Workflow permissions

## 📱 Custom Domain (Optional)

### Using Custom Domain

If you want to use your own domain (e.g., `docs.iquivity.ai`):

1. **Configure DNS:**
   - Add CNAME record pointing to `your-username.github.io`

2. **Update GitHub Settings:**
   - Settings → Pages
   - Custom domain: `docs.iquivity.ai`
   - Save

3. **Update mkdocs.yml:**
   ```yaml
   site_url: https://docs.iquivity.ai/
   ```

4. **Create CNAME file:**
   ```bash
   echo "docs.iquivity.ai" > docs/CNAME
   ```

5. **Commit and push:**
   ```bash
   git add docs/CNAME mkdocs.yml
   git commit -m "Add custom domain"
   git push
   ```

### SSL Certificate

GitHub Pages automatically provides HTTPS for:
- `*.github.io` domains (immediate)
- Custom domains (may take 24-48 hours)

Enable in: Settings → Pages → Enforce HTTPS ✓

## 🎯 Best Practices

### Version Control

✅ **Do:**
- Commit documentation updates regularly
- Use meaningful commit messages
- Create branches for major updates
- Review changes before merging

❌ **Don't:**
- Commit the `site/` directory (it's built automatically)
- Include sensitive information in docs
- Make direct commits to main for large changes

### Documentation Maintenance

**Regular Updates:**
- Review and update screenshots
- Keep feature documentation current
- Fix broken links
- Update version numbers

**Quality Checks:**
- Test all examples
- Verify links work
- Check for typos
- Ensure consistent formatting

## 📞 Support

### Getting Help

**Documentation Issues:**
- Check troubleshooting section above
- Review GitHub Actions logs
- Search GitHub Pages documentation

**Platform Issues:**
- Email: support@iquivity.ai
- Review platform documentation

**Technical Support:**
- Create issue in repository
- Include error logs and steps to reproduce

## 🔗 Useful Links

- **MkDocs Documentation**: https://www.mkdocs.org/
- **Material Theme**: https://squidfunk.github.io/mkdocs-material/
- **GitHub Pages**: https://docs.github.com/en/pages
- **GitHub Actions**: https://docs.github.com/en/actions

## ✅ Deployment Checklist

Before going live:

- [ ] Updated `site_url` in `mkdocs.yml`
- [ ] All markdown files are error-free
- [ ] Images are properly linked
- [ ] Navigation structure is complete
- [ ] Tested locally with `mkdocs serve`
- [ ] Repository is created on GitHub
- [ ] First commit pushed successfully
- [ ] GitHub Actions workflow completed
- [ ] GitHub Pages is enabled
- [ ] Documentation is accessible at GitHub Pages URL
- [ ] All links work correctly
- [ ] Documentation reviewed for accuracy

## 🎉 Success!

Once deployed, your documentation will be:
- ✅ Automatically updated on every push
- ✅ Searchable with full-text search
- ✅ Mobile-responsive
- ✅ Accessible worldwide
- ✅ Fast and reliable

Share your documentation URL with your team and users!

---

**Last Updated:** December 2025
