# AI Chat Pro Settings

Configure and customize your AI Chat Pro experience with categories, templates, and custom chatbot training.

---

## Overview

AI Chat Pro Settings allows you to:

- **Chat Categories** - Organize chatbots into categories
- **Chat Templates** - Create and manage pre-configured chatbot templates
- **Chatbot Training** - Train custom chatbots on your own data

---

## Accessing Chat Settings

**Navigate to Settings:**

1. Open **AI Chat Pro** from the main navigation
2. Click **"AI Chat Settings"** in the sidebar
3. Choose from available options:
   - AI Chat Categories
   - AI Chat Templates
   - Chatbot Training

---

## Chat Categories

### What are Chat Categories?

Chat Categories help you organize your chatbot templates into logical groups for easier management and discovery.

### Managing Categories

**Category Dashboard:**

```
Chat Categories
Manage Chat Categories                                [Add Category]

NAME                      ACTION
Customer Support          [✏️ Edit] [✖ Delete]
Entertainment            [✏️ Edit] [✖ Delete]
Learning & Education     [✏️ Edit] [✖ Delete]
Personal Assistants      [✏️ Edit] [✖ Delete]
Personal Development     [✏️ Edit] [✖ Delete]
Sales & Marketing        [✏️ Edit] [✖ Delete]
```

### Creating a Category

**To Add a New Category:**

1. Click **"Add Category"** button
2. Enter category name
3. Save

**Category Name Examples:**
- Customer Support
- Entertainment
- Learning & Education
- Personal Assistants
- Personal Development
- Sales & Marketing
- Technical & IT
- Healthcare & Wellness
- Business & Finance
- Creative & Design

### Editing Categories

**To Modify a Category:**

1. Click the **Edit icon (✏️)** next to the category
2. Update the category name
3. Save changes

### Deleting Categories

**To Remove a Category:**

1. Click the **Delete icon (✖)** next to the category
2. Confirm deletion

!!! warning "Category Deletion"
    Deleting a category does not delete the templates within it. Templates will become uncategorized and can be reassigned to other categories.

### Best Practices for Categories

**Organize by Purpose:**
```
By Function:
├─ Customer Support
├─ Sales & Marketing
├─ Technical Support
└─ Administrative Tasks

By Department:
├─ HR & Recruiting
├─ Finance & Accounting
├─ IT & Development
└─ Operations

By User Type:
├─ Executive Assistants
├─ Personal Productivity
├─ Team Collaboration
└─ Learning & Development
```

**Tips:**
- Keep category names short and descriptive
- Use consistent naming conventions
- Group related templates together
- Don't create too many categories (5-10 is ideal)
- Review and consolidate regularly

---

## Chat Templates

### What are Chat Templates?

Chat Templates are pre-configured chatbot personas with specific roles, instructions, and behaviors. They provide quick access to specialized AI assistants without needing to configure them each time.

### Template Dashboard

**Template List View:**

```
Chat Templates                                        [Add Template]

TEMPLATE NAME        DESCRIPTION              USER    ROLE              PLAN  UPDATED AT
Career Counselor     Personal Career...       System  Career Counselor  VIP   16.5.2023 03:39:11
Chat Image          Image Generator          System  Image Generator   VIP   16.5.2023 03:39:11
Cybersecurity...    Cybersecurity Expert     System  Cybersecurity...  VIP   16.5.2023 03:39:11
Default AI Chat Bot Default                  System  default           VIP   16.5.2023 03:39:11
Event Planner       Event Planner            System  Event Planner     VIP   16.5.2023 03:34:57
Finance Expert      Personal Finance...      System  Finance Expert    VIP   16.5.2023 03:39:11
```

### System Templates

**Pre-Built Templates Available:**

**Personal Assistants:**
- **Default AI Chat Bot** - General-purpose assistant
- **Career Counselor** - Personal career guidance
- **Finance Expert** - Personal finance advice
- **Time Management** - Productivity consultant
- **Event Planner** - Event planning assistance

**Specialized Experts:**
- **Cybersecurity Expert** - Security best practices
- **Nutritionist** - Diet and nutrition advice
- **Language Tutor** - Language learning help

**Creative Tools:**
- **Chat Image** - Image generation assistant

**Template Properties:**
- **Template Name** - Display name of the chatbot
- **Template Description** - Brief description of capabilities
- **User** - Creator (System or custom)
- **Role** - Functional role/persona
- **Plan** - Required subscription tier
- **Updated At** - Last modification date

### Creating Custom Templates

**To Add a New Template:**

1. Click **"Add Template"** button
2. Fill in template details:
   - **Template Name** - e.g., "Marketing Writer"
   - **Description** - e.g., "Specialist in marketing content creation"
   - **Role** - e.g., "Marketing Expert"
   - **Category** - Select from dropdown
   - **Instructions** - Detailed prompt for AI behavior
   - **Model** - Choose AI model
   - **Plan Level** - Set access requirements
3. Save template

**Template Instructions Example:**

```
Role: Marketing Content Writer

You are an expert marketing content writer specializing in:
- Blog posts and articles
- Social media content
- Email marketing campaigns
- Landing page copy
- Ad copy and CTAs

Style Guide:
- Tone: Professional yet conversational
- Use persuasive language
- Include clear calls-to-action
- Focus on benefits over features
- Keep sentences concise

Always ask clarifying questions about:
- Target audience
- Brand voice
- Content goals
- Key messages
```

### Editing Templates

**To Modify a Template:**

1. Click the **Edit icon (✏️)** next to the template
2. Update any fields:
   - Name
   - Description
   - Role
   - Category
   - Instructions
   - Model selection
3. Save changes

**When to Edit:**
- Improve template instructions
- Update for new use cases
- Refine AI behavior
- Change model assignment
- Update category

### Deleting Templates

**To Remove a Template:**

1. Click the **Delete icon (✖)** next to the template
2. Confirm deletion

!!! warning "Template Deletion"
    Deleting a template removes it from the available chatbot list. This action cannot be undone. System templates cannot be deleted.

### Using Templates

**To Use a Template:**

1. Open AI Chat Pro
2. Click the chatbot selector dropdown
3. Choose your desired template
4. Start chatting!

The AI will follow the template's instructions and behave according to its configured role.

---

## Chatbot Training

### What is Chatbot Training?

Chatbot Training allows you to create custom AI assistants trained on your own data (websites, PDFs, documents) to make your AI responses exclusive to your content.

### Training Dashboard

**Chatbot List:**

```
Chatbot Training                                      [Add Template]
Train iQuivity on your own data (website or PDF) and make your AI content exclusive.

NAME              STATUS         CREATED        MODEL         ACTIONS
Untitled chatbot  Not Trained    7 months ago   gpt-4o-mini   [✨ Train] [✖ Delete]
Untitled chatbot  Not Trained    7 months ago   gpt-4o-mini   [✨ Train] [✖ Delete]
Untitled chatbot  Not Trained    6 months ago   gpt-4o-mini   [✨ Train] [✖ Delete]
Zerify chatbot    Trained        4 months ago   gpt-4o-mini   [✨ Train] [✖ Delete]
```

**Chatbot Properties:**
- **Name** - Chatbot identifier
- **Status** - Training status (Trained / Not Trained)
- **Created** - Creation date
- **Model** - AI model used (e.g., gpt-4o-mini)
- **Actions** - Train or delete options

### Creating a Custom Chatbot

**Step 1: Create New Chatbot**

1. Click **"Add Template"** button
2. Enter chatbot name (or use default "Untitled chatbot")
3. Select AI model
4. Proceed to training

**Step 2: Select Training Source**

Choose how to train your chatbot:

**Available Sources:**
- **Website** - Scrape content from websites
- **PDF, XLSX, CSV** - Upload documents
- **Text** - Enter custom text content
- **Q&A** - Create question-answer pairs

### Training Method 1: Website

**To Train from Website:**

1. Select **"Website"** tab
2. Choose training mode:
   - **Website** - Full site scraping
   - **Single URL** - Specific page only

**Website Training:**
```
1. Add URL
   [https://example.com]                    [🔄]

2. Select Pages                         [Select All]

   [Start crawling to discover pages...]

3. [Train GPT]
```

**Process:**
1. Enter your website URL
2. Click refresh icon to crawl
3. System discovers all pages
4. Select which pages to include
5. Click **"Train GPT"** to start training

**What Gets Scraped:**
- Page text content
- Headers and subheadings
- Lists and bullet points
- Main body content

**What's Excluded:**
- Navigation menus
- Footers
- Sidebar content
- Advertisements
- JavaScript/CSS code

**Best Practices:**
- Select relevant pages only
- Exclude login/admin pages
- Include FAQ and help content
- Update training when site changes

### Training Method 2: Documents (PDF, XLSX, CSV)

**To Train from Documents:**

1. Select **"PDF, XLSX, CSV"** tab
2. Upload your files
3. System extracts content
4. Review extracted data
5. Train chatbot

**Supported Formats:**
- **PDF** - Text-based PDFs (not scanned images)
- **Excel (XLSX)** - Spreadsheet data
- **CSV** - Comma-separated values

**File Requirements:**
- Max file size: 25MB per file
- Max pages (PDF): 500 pages
- Text must be extractable (not images)

**Use Cases:**
- Product catalogs (PDF)
- Price lists (Excel/CSV)
- Technical documentation (PDF)
- Knowledge bases (PDF)
- Data tables (Excel/CSV)

### Training Method 3: Text

**To Train with Custom Text:**

1. Select **"Text"** tab
2. Paste or type your content
3. Format with markdown if needed
4. Train chatbot

**What to Include:**
- Company information
- Product descriptions
- Policies and procedures
- Brand guidelines
- FAQ content
- Technical specifications

**Example Text Training:**
```
Company: TechCorp Solutions
Industry: B2B SaaS

Products:
1. CloudSync Pro - Enterprise file synchronization
   - Pricing: $99/user/month
   - Features: Real-time sync, 1TB storage, API access

2. DataVault - Secure backup solution
   - Pricing: $49/user/month
   - Features: Automated backups, encryption, 500GB storage

Support: support@techcorp.com
Sales: sales@techcorp.com
Hours: Monday-Friday, 9 AM - 5 PM EST
```

### Training Method 4: Q&A

**To Train with Q&A Pairs:**

1. Select **"Q&A"** tab
2. Create question-answer pairs
3. Add multiple pairs
4. Train chatbot

**Q&A Format:**
```
Question: What are your business hours?
Answer: We're open Monday-Friday, 9 AM to 5 PM EST.
Closed on weekends and major holidays.

Question: What payment methods do you accept?
Answer: We accept Visa, MasterCard, American Express,
PayPal, and wire transfers for enterprise accounts.

Question: How long does shipping take?
Answer: Domestic shipping: 3-5 business days
International: 7-14 business days
Express shipping available at checkout.
```

**Q&A Best Practices:**
- Create 20-50 Q&A pairs minimum
- Cover common customer questions
- Use natural language
- Keep answers concise and clear
- Include specific details
- Update regularly

### Training Status

**Not Trained:**
- Chatbot created but no data added yet
- Cannot be used for conversations
- Needs training data to function

**Trained:**
- Has training data loaded
- Ready to use in conversations
- Will respond based on trained content
- Can be retrained with new data

### Using Trained Chatbots

**To Use Your Custom Chatbot:**

1. Complete training process
2. Go to AI Chat Pro main interface
3. Select your custom chatbot from dropdown
4. Start chatting with your trained assistant

**Your chatbot will:**
- Answer based on your training data
- Stay within the scope of provided content
- Provide more accurate, specific responses
- Represent your brand/company knowledge

### Retraining Chatbots

**To Update Training:**

1. Click **Train icon (✨)** next to chatbot
2. Add new content or modify existing
3. Re-run training process
4. Updated chatbot ready to use

**When to Retrain:**
- Add new products/services
- Update policies
- Correct inaccurate information
- Expand knowledge base
- Improve response quality

### Managing Trained Chatbots

**Editing Chatbot:**
- Update name
- Change AI model
- Modify training data
- Add/remove content sources

**Deleting Chatbot:**
- Click delete icon
- Confirm deletion
- All training data removed
- Cannot be recovered

---

## Use Cases

### Customer Support Chatbot

**Setup:**
1. Create category: "Customer Support"
2. Train chatbot on:
   - Support documentation
   - FAQ page
   - Common issues (Q&A)
   - Product manuals (PDF)

**Result:**
- Instant support responses
- 24/7 availability
- Consistent answers
- Reduced support tickets

### Sales Assistant

**Setup:**
1. Create category: "Sales & Marketing"
2. Train chatbot on:
   - Product catalog
   - Pricing information
   - Sales scripts (Q&A)
   - Case studies (PDF)

**Result:**
- Quick product information
- Pricing details on demand
- Lead qualification
- Sales enablement

### Company Knowledge Base

**Setup:**
1. Create category: "Internal Knowledge"
2. Train chatbot on:
   - Company policies (PDF)
   - Employee handbook
   - Procedures documentation
   - Department FAQs

**Result:**
- Employee self-service
- Quick policy lookup
- Onboarding assistance
- Process guidance

### Industry Expert

**Setup:**
1. Create category: "Industry Expertise"
2. Train chatbot on:
   - Industry reports (PDF)
   - Research papers
   - Best practices
   - Technical standards

**Result:**
- Expert-level responses
- Industry-specific knowledge
- Competitive intelligence
- Research assistance

---

## Best Practices

### Category Organization

**DO:**
- ✅ Create 5-10 main categories
- ✅ Use clear, descriptive names
- ✅ Group related templates
- ✅ Review and consolidate regularly

**DON'T:**
- ❌ Create too many categories
- ❌ Use vague category names
- ❌ Mix unrelated templates
- ❌ Duplicate categories

### Template Creation

**DO:**
- ✅ Write detailed instructions
- ✅ Define clear roles
- ✅ Specify tone and style
- ✅ Test before deploying
- ✅ Update regularly

**DON'T:**
- ❌ Leave instructions vague
- ❌ Mix multiple roles
- ❌ Skip testing
- ❌ Create duplicate templates

### Chatbot Training

**DO:**
- ✅ Use high-quality source data
- ✅ Train on relevant content only
- ✅ Test chatbot responses
- ✅ Update training regularly
- ✅ Verify accuracy

**DON'T:**
- ❌ Include outdated information
- ❌ Mix unrelated content
- ❌ Skip quality review
- ❌ Neglect retraining
- ❌ Use poor quality sources

---

## Troubleshooting

### Common Issues

**Problem: Category won't delete**
- **Cause**: May have system protection or templates assigned
- **Solution**: Move templates to other categories first, then delete

**Problem: Template not appearing**
- **Cause**: Wrong plan level or not saved
- **Solution**: Check plan requirements, verify template is saved

**Problem: Training failed**
- **Cause**: Invalid URL, corrupted file, or file too large
- **Solution**: Check URL accessibility, verify file format, reduce file size

**Problem: Chatbot gives generic responses**
- **Cause**: Insufficient training data
- **Solution**: Add more comprehensive training content

**Problem: Can't find trained chatbot**
- **Cause**: Not saved as template or training incomplete
- **Solution**: Complete training process, save chatbot properly

---

## Additional Resources

<div class="grid cards" markdown>

-   :material-robot:{ .lg .middle } __AI Chat Pro Overview__

    ---

    Learn about all AI Chat Pro features

    [:octicons-arrow-right-24: Overview](overview.md)

-   :material-chat:{ .lg .middle } __Using AI Chat Pro__

    ---

    Master the chat interface

    [:octicons-arrow-right-24: Usage Guide](usage.md)

-   :material-message-text:{ .lg .middle } __Managing Conversations__

    ---

    Organize and share conversations

    [:octicons-arrow-right-24: Conversations](conversations.md)

</div>

---

**Previous:** [← Conversations](conversations.md) | **Up:** [AI Chat Pro Overview](overview.md)

---

**Last Updated:** December 2025
