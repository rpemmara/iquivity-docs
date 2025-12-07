# GitHub Pages Setup - Next Steps

Your iQuivity documentation is ready to be deployed to GitHub Pages! Follow these steps to make it publicly accessible.

## ✅ What's Been Completed

✓ Git repository initialized
✓ Documentation files organized in `docs/` directory
✓ MkDocs configuration ready (`mkdocs.yml`)
✓ GitHub Actions workflow created (`.github/workflows/deploy-docs.yml`)
✓ Python dependencies listed (`requirements.txt`)
✓ Initial commit created with all documentation
✓ .gitignore configured to exclude build files

## 📋 What You Need to Do Next

### Step 1: Create GitHub Repository

1. Go to https://github.com/new
2. Fill in repository details:
   - **Repository name**: `iquivity-docs` (or your choice)
   - **Description**: "iQuivity Platform Documentation"
   - **Visibility**: **Public** (required for free GitHub Pages)
   - **DO NOT** initialize with README, .gitignore, or license (we already have them)
3. Click **"Create repository"**

### Step 2: Update Site URL

1. Open `mkdocs.yml` in your editor
2. Find lines 4-6:
   ```yaml
   site_url: https://[your-github-username].github.io/[your-repo-name]/
   # Change the above URL to match your GitHub Pages URL after deployment
   # Format: https://USERNAME.github.io/REPOSITORY-NAME/
   ```
3. Replace with your actual GitHub username and repository name:
   ```yaml
   site_url: https://your-username.github.io/iquivity-docs/
   ```
4. Save the file
5. Commit the change:
   ```bash
   git add mkdocs.yml
   git commit -m "Update site URL for GitHub Pages"
   ```

### Step 3: Push to GitHub

Run these commands in your terminal:

```bash
# Add your GitHub repository as remote (replace with YOUR repository URL)
git remote add origin https://github.com/YOUR-USERNAME/iquivity-docs.git

# Rename branch to 'main' (GitHub's default)
git branch -M main

# Push to GitHub
git push -u origin main
```

**Important**: Replace `YOUR-USERNAME` and `iquivity-docs` with your actual values!

### Step 4: Configure GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. In the left sidebar, click **"Pages"**
4. Under **"Build and deployment"**:
   - **Source**: Select **"GitHub Actions"**
5. The workflow will automatically start

### Step 5: Wait for Deployment

1. Click on the **"Actions"** tab in your repository
2. You'll see "Deploy Documentation" workflow running
3. Wait for it to complete (usually 1-3 minutes)
4. Look for a green checkmark ✓ indicating success

### Step 6: Access Your Documentation

Once the workflow completes successfully, your documentation will be live at:

```
https://YOUR-USERNAME.github.io/iquivity-docs/
```

Replace `YOUR-USERNAME` with your GitHub username.

## 🎯 Quick Commands Reference

### Initial Push to GitHub
```bash
# Configure git user (if not already done)
git config user.name "Your Name"
git config user.email "your.email@example.com"

# Add remote and push
git remote add origin https://github.com/YOUR-USERNAME/iquivity-docs.git
git branch -M main
git push -u origin main
```

### Update Documentation (After Initial Setup)
```bash
# Make your changes to files in docs/ directory
# Then commit and push:

git add .
git commit -m "Updated documentation"
git push
```

The documentation will automatically rebuild and deploy in 1-2 minutes!

## 📁 Repository Structure

```
iquivity-docs/
├── .github/
│   └── workflows/
│       └── deploy-docs.yml          # Auto-deployment workflow
├── docs/                            # All documentation content
│   ├── index.md                     # Homepage
│   ├── getting-started/             # Getting started guides
│   ├── features/                    # Feature documentation
│   │   ├── ai-writer.md            # AI Content tools
│   │   ├── ai-images.md            # AI Image tools
│   │   └── ai-videos.md            # AI Video tools
│   ├── chatbots/                    # Chatbot documentation
│   │   ├── iq-bot/
│   │   ├── ai-bot/
│   │   └── chat-pro/
│   ├── marketing/                   # Marketing tools
│   └── account/                     # Account management
├── mkdocs.yml                       # MkDocs configuration
├── requirements.txt                 # Python dependencies
├── .gitignore                       # Git ignore rules
├── DOCS_README.md                  # Documentation overview
├── DEPLOYMENT_GUIDE.md             # Detailed deployment guide
├── QUICK_START.md                  # 5-minute quick start
└── GITHUB_PAGES_SETUP.md           # This file
```

## 🔍 What Happens When You Push?

1. **GitHub Actions Triggers**
   - Runs automatically on push to `main` branch
   - Uses Ubuntu Linux environment

2. **Setup Phase**
   - Checks out your code
   - Installs Python 3.x
   - Installs MkDocs and Material theme
   - Installs awesome-pages plugin

3. **Build Phase**
   - Reads `mkdocs.yml` configuration
   - Processes all Markdown files in `docs/`
   - Generates static HTML site
   - Applies Material theme styling

4. **Deploy Phase**
   - Creates/updates `gh-pages` branch
   - Pushes built site to `gh-pages` branch
   - GitHub Pages serves from `gh-pages` branch

5. **Result**
   - Your documentation is live!
   - Accessible at your GitHub Pages URL
   - Future pushes trigger automatic updates

## 🛠️ Local Development (Optional)

To preview documentation locally before pushing:

```bash
# Install dependencies
pip install -r requirements.txt

# Start local server
mkdocs serve

# Open browser to http://127.0.0.1:8000
```

Make changes and see them live! Press Ctrl+C to stop the server.

## 📊 Documentation Statistics

Your completed documentation includes:

**AI Content Tools:** 4 complete guides
- AI Writer
- AI Editor
- AI Article Wizard
- AI ReWriter

**AI Image Tools:** 7 complete guides
- Creative Suite
- AI Image Editor
- AI Image
- AI Realtime Image
- AI Product Shot
- AI Chat Image
- AI Vision

**AI Video Tools:** 5 complete guides
- AI Video To Video
- AI Video Pro
- AI Persona
- AI Video
- AI Avatar

**Chatbots:** 3 complete sections
- IQ Bot (4 pages)
- AI Bot (7 pages)
- AI Chat Pro (4 pages)

**Total:** 50+ documentation pages, ~31,000+ lines of content

## 🚨 Troubleshooting

### Issue: Push Rejected

**Error**: `! [rejected] main -> main (fetch first)`

**Solution**:
```bash
git pull origin main --rebase
git push -u origin main
```

### Issue: Workflow Fails

**Check**:
1. Go to Actions tab
2. Click failed workflow
3. Read error logs
4. Common fix: Verify `requirements.txt` has all dependencies

### Issue: 404 Page Not Found

**Solutions**:
1. Wait 5-10 minutes after first deployment
2. Check Settings → Pages → ensure source is "GitHub Actions"
3. Verify `site_url` in `mkdocs.yml` matches your actual URL
4. Clear browser cache

### Issue: Images Not Loading

**Check**:
1. Images are in `docs/assets/images/` directory
2. Image paths in markdown use relative paths
3. Image files were committed to git

## 🎨 Customization Options

### Change Theme Colors

Edit `mkdocs.yml`:
```yaml
theme:
  palette:
    primary: indigo  # Change to: blue, red, green, etc.
    accent: blue     # Change to: orange, pink, etc.
```

### Add Your Logo

1. Place logo in `docs/assets/images/logo.svg`
2. Already configured in `mkdocs.yml`

### Update Social Links

Edit `mkdocs.yml`:
```yaml
extra:
  social:
    - icon: fontawesome/brands/twitter
      link: https://twitter.com/yourhandle
```

## 📞 Need Help?

**Read the guides:**
- **Quick Start**: [QUICK_START.md](QUICK_START.md) - 5-minute guide
- **Full Guide**: [DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md) - Complete instructions
- **Documentation**: [DOCS_README.md](DOCS_README.md) - Documentation overview

**External Resources:**
- MkDocs: https://www.mkdocs.org/
- Material Theme: https://squidfunk.github.io/mkdocs-material/
- GitHub Pages: https://docs.github.com/en/pages

## ✅ Pre-Deployment Checklist

Before pushing to GitHub:

- [ ] Created GitHub repository (public)
- [ ] Updated `site_url` in `mkdocs.yml` with YOUR username and repo name
- [ ] Committed the mkdocs.yml change
- [ ] Have your repository URL ready
- [ ] Know your GitHub username

Ready to deploy? Run the commands in **Step 3** above!

## 🎉 After Deployment

Once your documentation is live:

1. **Share the URL** with your team
2. **Bookmark** the documentation site
3. **Set up** a custom domain (optional, see DEPLOYMENT_GUIDE.md)
4. **Update** documentation as needed - changes deploy automatically!

## 📝 Example Repository URLs

**Your repository**: `https://github.com/YOUR-USERNAME/iquivity-docs`
**Your documentation**: `https://YOUR-USERNAME.github.io/iquivity-docs/`

Example (if username is "johndoe"):
- Repository: `https://github.com/johndoe/iquivity-docs`
- Documentation: `https://johndoe.github.io/iquivity-docs/`

---

**Ready to deploy?** Follow Steps 1-6 above and your documentation will be live in minutes!

**Questions?** Check DEPLOYMENT_GUIDE.md for detailed troubleshooting.

**Last Updated**: December 2025
