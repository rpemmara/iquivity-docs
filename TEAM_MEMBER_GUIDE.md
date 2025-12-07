# Team Member Guide - iQuivity Documentation

Welcome to the iQuivity documentation team! This guide will help you get started with editing and updating the documentation.

## 🚀 Quick Start

### Prerequisites
- GitHub account
- Git installed on your computer
- Text editor (VS Code, Sublime, etc.)
- Python 3.x (for local preview - optional)

---

## 📥 Initial Setup

### 1. Accept Repository Invitation
You'll receive an email invitation to collaborate on the repository. Click the link and accept.

### 2. Clone the Repository
```bash
# Clone the repository to your computer
git clone https://github.com/rpemmara/iquivity-docs.git

# Navigate into the directory
cd iquivity-docs
```

### 3. Install Dependencies (Optional - for local preview)
```bash
# Install MkDocs and theme
pip install -r requirements.txt
```

---

## ✏️ Making Changes

### Edit Documentation Files

All documentation is in the `docs/` directory:

```
docs/
├── index.md                    # Homepage
├── getting-started/            # Getting started guides
├── features/                   # Feature documentation
│   ├── ai-writer.md           # AI Content tools
│   ├── ai-images.md           # AI Image tools
│   └── ai-videos.md           # AI Video tools
├── chatbots/                  # Chatbot guides
│   ├── iq-bot/
│   ├── ai-bot/
│   └── chat-pro/
├── marketing/                 # Marketing tools
└── account/                   # Account management
```

**Edit files using any text editor:**
- VS Code (recommended)
- Sublime Text
- Atom
- Even Notepad!

**Files are in Markdown format (.md)**

---

## 🔄 Publishing Changes

### Simple 3-Step Process

#### 1. **Make Your Changes**
Edit the Markdown files in the `docs/` directory.

#### 2. **Commit Your Changes**
```bash
# Add all changed files
git add .

# Commit with a descriptive message
git commit -m "Updated AI Writer features section"
```

#### 3. **Push to GitHub**
```bash
git push
```

**That's it!** GitHub will automatically:
- Build the documentation (1-2 minutes)
- Deploy to https://rpemmara.github.io/iquivity-docs/
- Send you an email if the build fails

---

## 👀 Preview Before Publishing (Optional)

To preview your changes locally before pushing:

```bash
# Start local server
mkdocs serve

# Open browser to: http://127.0.0.1:8000
```

Make changes to files - the preview updates automatically!
Press `Ctrl+C` to stop the server.

---

## 📝 Markdown Quick Reference

### Headers
```markdown
# H1 Header
## H2 Header
### H3 Header
```

### Text Formatting
```markdown
**Bold text**
*Italic text*
`Code text`
```

### Links
```markdown
[Link text](url)
[Internal link](../folder/page.md)
```

### Lists
```markdown
- Bullet point
- Another point

1. Numbered item
2. Another item
```

### Code Blocks
````markdown
```python
def hello():
    print("Hello, world!")
```
````

### Images
```markdown
![Alt text](../assets/images/image.png)
```

### Admonitions (Tips, Warnings, etc.)
```markdown
!!! tip "Helpful Tip"
    This is a tip box

!!! warning "Important Warning"
    Pay attention to this

!!! note "Note"
    Additional information
```

---

## 🎨 Documentation Style Guide

### Writing Guidelines

**DO:**
- ✅ Use clear, concise language
- ✅ Include step-by-step instructions
- ✅ Add screenshots where helpful
- ✅ Use consistent formatting
- ✅ Test all examples
- ✅ Write in active voice

**DON'T:**
- ❌ Use jargon without explanation
- ❌ Write long paragraphs (break them up)
- ❌ Forget to update screenshots
- ❌ Leave broken links
- ❌ Use vague instructions

### Formatting Standards

**File Names:**
- Use lowercase
- Use hyphens, not spaces: `ai-writer.md` ✅ not `AI Writer.md` ❌

**Headers:**
- Main title: `# Title` (only one per page)
- Sections: `## Section`
- Subsections: `### Subsection`

**Screenshots:**
- Place in `docs/assets/images/`
- Use descriptive names: `ai-writer-interface.png`
- Optimize file size (keep under 500KB)

---

## 🔄 Workflow Best Practices

### Before Making Changes

1. **Pull latest changes:**
   ```bash
   git pull
   ```

2. **Create a branch for major changes (optional):**
   ```bash
   git checkout -b update-ai-features
   ```

### After Making Changes

1. **Test locally** (if you have MkDocs installed):
   ```bash
   mkdocs serve
   ```

2. **Check for broken links**

3. **Commit with descriptive messages:**
   ```bash
   # Good commit messages:
   git commit -m "Add AI Video Pro documentation"
   git commit -m "Fix broken links in AI Writer section"
   git commit -m "Update screenshots for Chat Pro"

   # Bad commit messages:
   git commit -m "updates"
   git commit -m "fixes"
   git commit -m "changes"
   ```

4. **Push to GitHub:**
   ```bash
   git push
   ```

---

## 🚨 Troubleshooting

### Problem: Can't Push Changes

**Error:** `Permission denied`

**Solution:**
- Ensure you've accepted the repository invitation
- Check you're logged into the correct GitHub account
- Verify you have Write permissions

### Problem: Build Fails

**Check:**
1. Go to: https://github.com/rpemmara/iquivity-docs/actions
2. Click the failed workflow
3. Read the error message
4. Common issues:
   - Syntax error in Markdown
   - Broken internal links
   - Missing images

**Fix:**
- Correct the error in your file
- Commit and push again

### Problem: Changes Don't Appear

**Wait:** Deployment takes 2-3 minutes

**Then:**
1. Clear browser cache
2. Do a hard refresh (Ctrl+F5 or Cmd+Shift+R)
3. Check Actions tab for deployment status

---

## 📂 Common Editing Tasks

### Add a New Page

1. **Create the file:**
   ```bash
   # Example: Add new AI tool documentation
   touch docs/features/ai-new-tool.md
   ```

2. **Add content to the file**

3. **Update navigation in `mkdocs.yml`:**
   ```yaml
   nav:
     - Features:
         - AI New Tool: features/ai-new-tool.md
   ```

4. **Commit and push**

### Update Existing Content

1. **Find the file** (e.g., `docs/features/ai-writer.md`)
2. **Edit the content**
3. **Save the file**
4. **Commit and push**

### Add Images

1. **Add image to** `docs/assets/images/`

2. **Reference in Markdown:**
   ```markdown
   ![Screenshot of AI Writer](../assets/images/ai-writer-screenshot.png)
   ```

3. **Commit and push** (including the image file)

---

## 👥 Collaboration Tips

### Multiple People Editing

**Before starting work:**
```bash
git pull
```

**Avoid conflicts:**
- Communicate with team about what you're editing
- Pull before making changes
- Push frequently
- Don't edit the same file simultaneously

**If you get a merge conflict:**
```bash
git pull
# Fix conflicts in your editor
git add .
git commit -m "Resolved merge conflict"
git push
```

---

## 📊 Monitoring Deployments

### Check Deployment Status

**Actions Tab:** https://github.com/rpemmara/iquivity-docs/actions

**Status Indicators:**
- 🟡 Yellow - Building/Deploying
- ✅ Green - Success
- ❌ Red - Failed (check error logs)

### View Live Site

**Documentation URL:** https://rpemmara.github.io/iquivity-docs/

Updates appear 2-3 minutes after pushing.

---

## 🎓 Learning Resources

**Markdown:**
- https://www.markdownguide.org/basic-syntax/

**MkDocs Material:**
- https://squidfunk.github.io/mkdocs-material/

**Git Basics:**
- https://git-scm.com/docs/gittutorial

**GitHub Docs:**
- https://docs.github.com/en

---

## 📞 Getting Help

**Documentation Issues:**
- Check the troubleshooting section above
- Ask the team lead
- Create an issue in the repository

**Git/GitHub Issues:**
- GitHub documentation
- Team lead
- Git documentation

---

## ✅ Quick Checklist

Before pushing changes:

- [ ] Pulled latest changes (`git pull`)
- [ ] Made edits to documentation
- [ ] Tested locally (if possible)
- [ ] Checked for typos and broken links
- [ ] Committed with descriptive message
- [ ] Pushed to GitHub
- [ ] Verified deployment succeeded

---

## 🎉 You're Ready!

You now have everything you need to contribute to the iQuivity documentation!

**Remember:**
- Pull before editing
- Commit with clear messages
- Push to deploy automatically
- Check Actions tab if something goes wrong

**Your changes help make iQuivity better for everyone!**

---

**Questions?** Contact the documentation team lead.

**Documentation URL:** https://rpemmara.github.io/iquivity-docs/
**Repository:** https://github.com/rpemmara/iquivity-docs
