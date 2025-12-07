# Training Your AI Bot

Learn how to train your AI Bot with knowledge from multiple sources to provide accurate, helpful responses to your visitors.

---

## Overview

Training your AI Bot is the most important step in creating an effective chatbot. The quality of your bot's responses directly depends on the quality and completeness of its training data.

!!! tip "Training Best Practice"
    The more comprehensive and accurate your training data, the better your bot will perform. Take time to provide thorough, well-organized information.

---

## Training Sources

AI Bot supports four different training methods:

<div class="grid cards" markdown>

-   :material-web:{ .lg .middle } __Website Content__

    ---

    Automatically scrape and import content from your website

    **Best For:** FAQ pages, product catalogs, documentation

-   :material-file-pdf-box:{ .lg .middle } __PDF Documents__

    ---

    Upload PDF files with relevant information

    **Best For:** Manuals, guides, policy documents

-   :material-comment-question:{ .lg .middle } __Q&A Pairs__

    ---

    Manually create question and answer pairs

    **Best For:** Specific responses, custom content

-   :material-text:{ .lg .middle } __Text Instructions__

    ---

    Add custom text blocks for specific topics

    **Best For:** General information, context

</div>

---

## Method 1: Website Content Training

### How Website Training Works

The AI Bot crawler visits your website and extracts text content from pages you specify. This content becomes part of the bot's knowledge base.

### Step-by-Step: Website Training

**1. Access Training Section**
- Go to your AI Bot dashboard
- Click **"Train"** or **"Knowledge Base"**
- Select **"Add Website"**

**2. Enter Website URL**
```
https://www.yourwebsite.com
```

**Configuration Options:**

| Option | Description | Recommendation |
|--------|-------------|----------------|
| **URL** | Starting page for crawler | Use homepage or main section |
| **Max Pages** | Limit pages to crawl | 50-100 for most sites |
| **Include Subdomains** | Crawl subdomains | Disable unless needed |
| **Depth** | How deep to follow links | 2-3 levels recommended |

**3. Select Pages to Include**

After crawling, you'll see a list of discovered pages:

```
☐ Homepage (/)
☐ About Us (/about)
☐ Products (/products)
  ☐ Product A (/products/a)
  ☐ Product B (/products/b)
☐ FAQ (/faq)
☐ Contact (/contact)
```

!!! warning "Selective Training"
    Don't include every page. Focus on pages with useful customer-facing information. Exclude:
    - Admin pages
    - Login/registration pages
    - Shopping cart pages
    - Privacy policy (unless answering privacy questions)

**4. Review Extracted Content**

Check the preview to ensure content is extracted correctly:

```
✅ Good: Clean text with proper formatting
❌ Poor: Code snippets, navigation menus, footers
```

**5. Start Training**

Click **"Import Selected Pages"** to begin training.

!!! info "Processing Time"
    Training time depends on content volume:
    - 10 pages: ~2-3 minutes
    - 50 pages: ~10-15 minutes
    - 100 pages: ~20-30 minutes

### Website Training Best Practices

**DO:**
- ✅ Train on FAQ pages first
- ✅ Include product/service information
- ✅ Use clear, well-written web content
- ✅ Update training when website changes
- ✅ Test bot responses after training

**DON'T:**
- ❌ Include duplicate content
- ❌ Train on poorly written pages
- ❌ Include navigation/footer text
- ❌ Scrape competitor websites
- ❌ Include outdated information

### Troubleshooting Website Training

**Problem: Content Not Extracted Properly**
- **Cause:** JavaScript-heavy website
- **Solution:** Use PDF upload or Q&A pairs instead

**Problem: Too Many Irrelevant Pages**
- **Cause:** Over-crawling
- **Solution:** Reduce depth limit, manually deselect pages

**Problem: Missing Important Pages**
- **Cause:** Pages not linked from crawl starting point
- **Solution:** Add individual URLs separately

---

## Method 2: PDF Document Training

### How PDF Training Works

Upload PDF files containing information you want the bot to know. The system extracts text and adds it to the knowledge base.

### Step-by-Step: PDF Training

**1. Prepare Your PDFs**

**Supported Files:**
- Format: PDF only (.pdf)
- Max Size: 25MB per file
- Max Pages: 500 pages
- Text: Must be text-based (not scanned images)

**2. Access Upload Section**
- Go to **"Train"** → **"Add PDF"**
- Click **"Choose File"** or drag and drop

**3. Upload and Process**

```
Uploading: product-manual.pdf (5.2 MB)
Processing... [=====>    ] 60%
Extracting text...
Completed! ✓
```

**4. Review Extracted Content**

Preview the extracted text:
- Check for formatting issues
- Verify important sections included
- Edit if necessary

**5. Add Metadata (Optional)**

```
Title: Product Manual
Category: Documentation
Description: Complete guide for Product XYZ
```

Metadata helps organize your knowledge base.

### What Makes a Good Training PDF?

**Ideal PDFs:**
- ✅ Clear, structured content
- ✅ Proper headings and sections
- ✅ Text-based (not scanned)
- ✅ Up-to-date information
- ✅ Customer-facing content

**PDFs to Avoid:**
- ❌ Scanned images without OCR
- ❌ Complex layouts with tables
- ❌ Password-protected files
- ❌ Internal-only documents
- ❌ Legal disclaimers

### PDF Training Best Practices

**Content Organization:**
```
Good Structure:
├─ Product Overview
├─ Features & Benefits
├─ Getting Started Guide
├─ Troubleshooting
└─ FAQ

Poor Structure:
└─ One long document with no headings
```

**Recommended PDFs:**
- Product manuals
- User guides
- FAQ compilations
- Policy documents
- Service catalogs
- Pricing sheets

### Troubleshooting PDF Training

**Problem: "Unable to Extract Text"**
- **Cause:** Scanned PDF or image-based
- **Solution:** Use OCR software first, or re-create as text PDF

**Problem: Extracted Text Garbled**
- **Cause:** Complex formatting, multiple columns
- **Solution:** Simplify PDF layout, or use Q&A pairs

**Problem: File Too Large**
- **Cause:** Exceeds 25MB limit
- **Solution:** Split into multiple files, compress PDF

---

## Method 3: Q&A Pairs Training

### How Q&A Training Works

Manually create question and answer pairs for specific responses you want the bot to give. This is the most precise training method.

### Step-by-Step: Q&A Training

**1. Access Q&A Section**
- Go to **"Train"** → **"Add Q&A"**
- Click **"Create New Q&A Pair"**

**2. Enter Question**

```
Question: What are your business hours?
```

**Tips for Writing Questions:**
- Use natural language
- Include variations (add synonyms)
- Think like a customer
- Be specific

**3. Enter Answer**

```
Answer: We're open Monday to Friday, 9 AM to 5 PM EST.
On Saturdays, we're open 10 AM to 2 PM.
We're closed on Sundays and major holidays.
```

**Tips for Writing Answers:**
- Be clear and concise
- Use complete sentences
- Include relevant details
- Keep friendly tone
- Add contact info if needed

**4. Add Variations (Optional)**

Different ways customers might ask the same question:

```
Variations:
- "When are you open?"
- "What time do you close?"
- "Are you open on weekends?"
- "Opening hours"
```

**5. Save and Test**

Click **"Save Q&A"** and test in preview mode.

### Q&A Training Examples

#### Customer Support Q&A

```
Q: How do I reset my password?
A: To reset your password:
1. Click "Forgot Password" on the login page
2. Enter your email address
3. Check your email for reset link
4. Follow the link and create a new password
Need help? Contact support@yourcompany.com

---

Q: What payment methods do you accept?
A: We accept:
• All major credit cards (Visa, MasterCard, Amex)
• PayPal
• Apple Pay
• Google Pay
For enterprise accounts, we also accept wire transfers.

---

Q: How long does shipping take?
A: Shipping times vary by location:
• US: 3-5 business days
• Canada: 5-7 business days
• International: 7-14 business days
Express shipping available at checkout.
```

#### Product Information Q&A

```
Q: What's the difference between Basic and Pro plans?
A: Basic Plan ($29/month):
• Up to 10 users
• 100 GB storage
• Email support

Pro Plan ($79/month):
• Unlimited users
• 1 TB storage
• Priority phone & email support
• Advanced analytics
• Custom integrations

---

Q: Is there a free trial?
A: Yes! We offer a 14-day free trial with full access
to Pro features. No credit card required.
Start your trial at: www.yoursite.com/trial
```

### Q&A Best Practices

**DO:**
- ✅ Create 20-50 Q&A pairs minimum
- ✅ Cover most common questions
- ✅ Use customer's language
- ✅ Keep answers concise (2-4 sentences)
- ✅ Update regularly

**DON'T:**
- ❌ Create duplicate Q&A pairs
- ❌ Use jargon or technical terms
- ❌ Give contradictory answers
- ❌ Leave answers incomplete
- ❌ Ignore spelling/grammar

### Organizing Q&A Pairs

**Create Categories:**
```
Account Management (15 Q&As)
├─ Login/Password
├─ Billing
└─ Account Settings

Products & Services (25 Q&As)
├─ Features
├─ Pricing
└─ Comparisons

Technical Support (20 Q&As)
├─ Troubleshooting
├─ Installation
└─ Integration

Shipping & Returns (10 Q&As)
```

---

## Method 4: Text Instructions Training

### How Text Training Works

Add custom text blocks with general information that doesn't fit into Q&A format.

### When to Use Text Instructions

**Use For:**
- Company overview
- General policies
- Brand voice guidelines
- Context setting
- Background information

**Example Text Instruction:**

```
Company Context:

We are TechCorp, a B2B SaaS company providing
cloud-based project management tools since 2015.

Our mission is to help teams collaborate more effectively.

Key values:
- Customer success first
- Innovation and simplicity
- Data security and privacy
- Responsive support

Target audience: Small to medium businesses
with 10-200 employees.

Tone: Professional but friendly, helpful, and clear.
```

### Text Training Best Practices

**Structure:**
```markdown
# Section Title

## Subsection

Key points:
- Point 1
- Point 2
- Point 3

Important: [Critical information]
```

**DO:**
- ✅ Provide context about your business
- ✅ Define brand voice
- ✅ Explain policies clearly
- ✅ Use bullet points
- ✅ Keep it organized

---

## Combining Training Methods

### Recommended Training Strategy

**1. Start with Website Training (Foundation)**
```
Import key pages:
- Homepage
- Products/Services
- FAQ
- About Us
```

**2. Add Q&A Pairs (Precision)**
```
Create 30-50 Q&As covering:
- Top 20 customer questions
- Product-specific queries
- Support procedures
```

**3. Upload PDFs (Depth)**
```
Add detailed documents:
- Product manual
- Policy documents
- User guides
```

**4. Add Text Instructions (Context)**
```
Provide background:
- Company overview
- Brand voice
- Special instructions
```

### Training Workflow

```
Week 1: Initial Setup
├─ Import website (key pages)
├─ Create 20 essential Q&As
└─ Test basic functionality

Week 2: Expansion
├─ Add 30 more Q&As
├─ Upload product PDFs
├─ Add text context
└─ Test comprehensively

Ongoing: Maintenance
├─ Update changed content
├─ Add new Q&As based on questions
├─ Refine unclear responses
└─ Monthly review
```

---

## Knowledge Base Management

### Viewing Your Knowledge Base

**Dashboard Overview:**
```
Total Training Sources: 45
├─ Website Pages: 15
├─ PDF Documents: 8
├─ Q&A Pairs: 20
└─ Text Instructions: 2

Last Updated: 2 days ago
Total Characters: 125,000
```

### Editing Training Data

**Update Content:**
1. Navigate to Knowledge Base
2. Find content to edit
3. Click **"Edit"**
4. Make changes
5. Save and retrain

!!! warning "Retraining Required"
    After editing, click **"Retrain Bot"** for changes to take effect.

### Deleting Training Data

**When to Delete:**
- Outdated information
- Incorrect content
- Duplicate entries
- Irrelevant material

**How to Delete:**
1. Select content to remove
2. Click **"Delete"**
3. Confirm deletion
4. Retrain bot

---

## Testing Your Training

### Preview Mode Testing

**Test Scenarios:**

**1. Common Questions**
```
Test: "What are your hours?"
Expected: Accurate business hours
Result: ✓ Correct response
```

**2. Product Information**
```
Test: "Tell me about your Pro plan"
Expected: Pro plan features and pricing
Result: ✓ Correct details
```

**3. Edge Cases**
```
Test: "Do you sell purple unicorns?"
Expected: Polite "I don't have that information"
Result: ✓ Handled gracefully
```

**4. Complex Queries**
```
Test: "I need help with password reset but email isn't working"
Expected: Password reset steps + escalation option
Result: Review and improve if needed
```

### Improving Bot Responses

**If Bot Gives Wrong Answer:**

1. **Identify the Gap**
   - What information was missing?
   - Was question misunderstood?

2. **Add Training Data**
   - Create specific Q&A pair
   - Add more context to existing content

3. **Test Again**
   - Verify improvement
   - Test related questions

4. **Monitor Performance**
   - Check analytics for similar questions
   - Update training as needed

---

## Advanced Training Techniques

### Using Training Data Effectively

**Hierarchy of Specificity:**
```
Most Specific (Highest Priority)
↓
Q&A Pairs ─────────► Direct question matches
↓
PDF Documents ─────► Detailed information
↓
Website Content ───► General information
↓
Text Instructions ─► Context & background
```

### Handling Multiple Topics

**Topic Organization:**

```
Sales Questions
├─ Use: Product PDFs + Pricing Q&As
└─ Style: Enthusiastic, helpful

Support Questions
├─ Use: Technical PDFs + Troubleshooting Q&As
└─ Style: Patient, step-by-step

General Inquiries
├─ Use: Website content + Company text
└─ Style: Friendly, informative
```

### Seasonal & Temporary Content

**Managing Time-Sensitive Info:**

```
Holiday Hours Q&A:
"What are your holiday hours this year?"

Update annually:
- December: Update for New Year
- July: Update for Independence Day
- etc.

Set reminders to update seasonal content!
```

---

## Training Limitations & Credits

### Content Limits

**Per Bot:**
- Website pages: Up to 200 pages
- PDF files: Up to 50 files (25MB each)
- Q&A pairs: Unlimited
- Text instructions: Up to 100,000 characters

### Credit Usage

**Training consumes credits based on content volume:**

| Source Type | Credit Cost |
|-------------|-------------|
| Website (per page) | 1-5 credits |
| PDF (per page) | 2-10 credits |
| Q&A pair | 0.5 credits |
| Text instruction | 1 credit per 1000 chars |

!!! info "Check Credits"
    Monitor your credit balance in Account Settings before training large datasets.

---

## Training Checklist

### Pre-Launch Training Checklist

Before deploying your bot, ensure:

**Content Coverage:**
- ☐ Top 20 customer questions answered
- ☐ Product/service information complete
- ☐ Contact information included
- ☐ Business hours specified
- ☐ Pricing information (if applicable)

**Quality Checks:**
- ☐ All responses tested in preview
- ☐ No contradictory information
- ☐ Grammar and spelling checked
- ☐ Tone matches brand voice
- ☐ Links and contact info verified

**Technical:**
- ☐ All training sources successfully imported
- ☐ Bot retrained after all updates
- ☐ Credit usage acceptable
- ☐ Performance tested on mobile

---

## Maintaining Your Training

### Regular Maintenance Schedule

**Weekly:**
- Review unanswered questions from analytics
- Add new Q&As for common queries

**Monthly:**
- Update changed product information
- Review and refresh outdated content
- Check for broken links in website training

**Quarterly:**
- Comprehensive training audit
- Remove obsolete content
- Major updates to PDFs/documentation

**Annually:**
- Complete training overhaul
- Website re-scrape
- Q&A pair review and consolidation

---

## Next Steps

Now that your bot is trained, move on to deployment:

**[→ Deploying Your AI Bot](deployment.md)**

Learn how to:
- Embed bot on your website
- Integrate with Facebook Messenger
- Connect to Telegram
- Set up WhatsApp integration
- Configure Human Agent handoff

---

**Previous:** [← Creating AI Bots](creating.md) | **Next:** [Deployment →](deployment.md)

---

**Last Updated:** December 2025
