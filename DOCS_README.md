# iQuivity Documentation

Comprehensive user documentation for the iQuivity platform - an all-in-one AI content generation and marketing automation platform.

## 📚 What's Documented

This documentation covers all major features of iQuivity:

### AI Content Generation
- **AI Writer** - Generate content from scratch with templates
- **AI Editor** - Edit and refine existing content
- **AI Article Wizard** - Step-by-step article creation
- **AI ReWriter** - Rewrite content in different styles

### AI Image Generation
- **Creative Suite** - Professional image generation
- **AI Image Editor** - Edit and enhance images
- **AI Image** - Text-to-image with multiple models
- **AI Realtime Image** - Real-time generation with style presets
- **AI Product Shot** - Professional product photography
- **AI Chat Image** - Conversational image generation
- **AI Vision** - Image analysis and OCR

### AI Video Generation
- **AI Video To Video** - Transform and enhance videos
- **AI Video Pro** - Text-to-video with multiple AI models (Sora, Google VEO, Luma Dream Machine, Kling, Minimax)
- **AI Persona** - Studio-quality videos with AI avatars in 130+ languages
- **AI Video** - URL-to-video and text-to-video
- **AI Avatar** - Custom avatar creation

### Chatbots & AI Assistants
- **IQ Bot** - Standalone chatbot mini-sites
- **AI Bot** - Website widget chatbots with custom training
- **AI Chat Pro** - Internal AI assistant with multiple providers (OpenAI, Anthropic, Google, Perplexity, DeepSeek, Grok, OpenRouter)

### Marketing Tools
- AI Social Media management
- Marketing Bot (Telegram, WhatsApp)
- AI Influencer tools

## 🚀 Viewing the Documentation

### Online (GitHub Pages)
The documentation is automatically deployed to GitHub Pages and accessible at:
```
https://[your-username].github.io/[repository-name]/
```

### Local Development

#### Prerequisites
- Python 3.x
- pip (Python package manager)

#### Setup

1. Clone the repository:
```bash
git clone [your-repository-url]
cd [repository-name]
```

2. Install MkDocs and dependencies:
```bash
pip install mkdocs-material
pip install mkdocs-awesome-pages-plugin
```

3. Serve documentation locally:
```bash
mkdocs serve
```

4. Open your browser to `http://127.0.0.1:8000`

#### Building Static Site

To build the static HTML site:
```bash
mkdocs build
```

The built site will be in the `site/` directory.

## 📖 Documentation Structure

```
docs/
├── index.md                          # Homepage
├── getting-started/                  # Getting Started guides
│   ├── introduction.md
│   ├── account-creation.md
│   └── dashboard.md
├── features/                         # Core features
│   ├── ai-writer.md                 # AI Content tools
│   ├── ai-images.md                 # AI Image tools
│   ├── ai-videos.md                 # AI Video tools
│   ├── file-management.md
│   ├── templates.md
│   └── collaboration.md
├── chatbots/                        # Chatbot documentation
│   ├── iq-bot/
│   ├── ai-bot/
│   └── chat-pro/
├── marketing/                       # Marketing tools
│   ├── social-media/
│   ├── marketing-bot/
│   └── ai-influencer/
└── account/                        # Account management
    ├── profile.md
    ├── security.md
    └── billing.md
```

## 🛠️ Technology Stack

- **MkDocs** - Static site generator
- **Material for MkDocs** - Modern documentation theme
- **GitHub Actions** - Automatic deployment
- **GitHub Pages** - Hosting

## 📝 Contributing

### Documentation Guidelines

1. **Markdown Format**: All documentation is written in Markdown
2. **Consistent Structure**: Follow existing page structures
3. **Screenshots**: Place in `docs/assets/images/`
4. **Code Examples**: Use fenced code blocks with language specification
5. **Admonitions**: Use Material theme admonitions (tip, warning, note, etc.)

### Making Changes

1. Edit documentation files in the `docs/` directory
2. Test locally with `mkdocs serve`
3. Commit changes to your branch
4. Push to GitHub - documentation will automatically deploy

### Style Guidelines

- Use clear, concise language
- Include step-by-step instructions where applicable
- Add screenshots for visual features
- Provide example prompts and outputs
- Use consistent formatting (see existing docs)

## 🔄 Automatic Deployment

Documentation is automatically deployed to GitHub Pages when changes are pushed to the `main` or `master` branch.

The deployment workflow (`.github/workflows/deploy-docs.yml`) will:
1. Install dependencies
2. Build the documentation
3. Deploy to GitHub Pages

## 📋 Configuration

### mkdocs.yml

The main configuration file includes:
- Site metadata (name, description, URL)
- Material theme configuration
- Navigation structure
- Markdown extensions
- Plugins (search, awesome-pages)
- Social links and analytics

### GitHub Pages Settings

After first deployment:
1. Go to your repository Settings
2. Navigate to "Pages"
3. Source should be set to "gh-pages" branch
4. Your site will be available at the GitHub Pages URL

## 🐛 Troubleshooting

### Local Server Issues

If `mkdocs serve` fails:
```bash
# Reinstall dependencies
pip install --upgrade mkdocs-material mkdocs-awesome-pages-plugin
```

### Build Errors

If build fails, check:
- All markdown files are properly formatted
- All links reference existing files
- No special characters in filenames
- Images are in correct directories

### Deployment Issues

If GitHub Actions deployment fails:
- Check workflow logs in the "Actions" tab
- Ensure repository has Pages enabled
- Verify workflow permissions in repository settings

## 📞 Support

For questions or issues:
- Create an issue in this repository
- Email: support@iquivity.ai
- Review existing documentation for examples

## 📄 License

Copyright © 2025 iQuivity. All rights reserved.

## 🔗 Links

- **Live Documentation**: [GitHub Pages URL will be here]
- **iQuivity Platform**: https://iquivity.ai
- **MkDocs**: https://www.mkdocs.org/
- **Material for MkDocs**: https://squidfunk.github.io/mkdocs-material/
