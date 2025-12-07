# Quick Start: Deploy to GitHub Pages

Get your iQuivity documentation live in 5 minutes!

## 🚀 Fast Track Deployment

### 1. Create GitHub Repository (2 minutes)

1. Go to https://github.com/new
2. Name: `iquivity-docs`
3. Public repository
4. **Don't** add README, .gitignore, or license
5. Click "Create repository"

### 2. Update Configuration (1 minute)

Edit `mkdocs.yml` line 4:

```yaml
# Change this:
site_url: https://[your-github-username].github.io/[your-repo-name]/

# To this (replace with YOUR username):
site_url: https://johndoe.github.io/iquivity-docs/
```

### 3. Push to GitHub (1 minute)

Run these commands in your project directory:

```bash
git add .
git commit -m "Initial commit: iQuivity documentation"
git remote add origin https://github.com/YOUR-USERNAME/iquivity-docs.git
git branch -M main
git push -u origin main
```

**Replace `YOUR-USERNAME` with your GitHub username!**

### 4. Enable GitHub Pages (30 seconds)

1. Go to your repository on GitHub
2. Settings → Pages
3. Source: "GitHub Actions"
4. Done!

### 5. Wait & Access (1-2 minutes)

1. Go to "Actions" tab
2. Wait for green checkmark ✓
3. Visit: `https://YOUR-USERNAME.github.io/iquivity-docs/`

## ✅ That's It!

Your documentation is now live and will automatically update when you push changes.

## 📝 Making Updates

Edit files in `docs/` folder, then:

```bash
git add .
git commit -m "Updated documentation"
git push
```

GitHub will automatically rebuild and deploy (1-2 minutes).

## 🆘 Need Help?

**Common Issues:**

1. **404 Error**: Wait 5 minutes, clear cache, check site_url
2. **Build fails**: Check Actions tab for error logs
3. **Can't push**: Check remote URL is correct

**Detailed Help:**
- See [DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md) for complete instructions
- See [DOCS_README.md](DOCS_README.md) for documentation structure

## 🎯 Next Steps

**Test Locally:**
```bash
pip install -r requirements.txt
mkdocs serve
# Visit http://127.0.0.1:8000
```

**Customize:**
- Add logo: `docs/assets/images/logo.svg`
- Update colors: Edit `mkdocs.yml` theme section
- Add pages: Create `.md` files in `docs/` and update navigation

**Share:**
Send your documentation URL to team members and users!

---

**Your URL will be:**
```
https://YOUR-USERNAME.github.io/iquivity-docs/
```

Replace `YOUR-USERNAME` with your actual GitHub username.
