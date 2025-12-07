# AI Bot Knowledge Base

Manage and organize your AI Bot's knowledge base articles for easy content updates and maintenance.

---

## Overview

The AI Bot Knowledge Base is a centralized repository where you can create, edit, and manage knowledge articles that train your AI Bot. This feature provides an organized way to maintain your bot's training data separate from the bot creation workflow.

---

## Accessing Knowledge Base

**Navigate to Knowledge Base:**

1. From the main dashboard, locate **"AI Bot Knowledge Base"** in the left-hand navigation
2. Click to open the Knowledge Base management page

**Dashboard View:**

The Knowledge Base shows a table with all your articles:

| Column | Description |
|--------|-------------|
| **ID** | Unique identifier for each article |
| **Title** | Article title/heading |
| **Excerpt** | Preview of article content |
| **Created At** | Date and time article was created |
| **Actions** | Edit (✏️) and Delete (✖) options |

---

## Creating Knowledge Base Articles

### Step 1: Add New Article

**Click "Add Article"** button (top-right corner)

### Step 2: Enter Article Details

**Article Title** (Required)
```
Example: "How to Improve Website Speed"
```

**Purpose:**
- Clear, descriptive heading
- Helps organize knowledge base
- Makes articles easy to find
- Used for article identification

**Best Practices:**
- ✅ Use descriptive, specific titles
- ✅ Keep titles concise (3-10 words)
- ✅ Use title case formatting
- ✅ Make titles searchable

**Article Content** (Required)

Enter the full content/body of your knowledge article.

**Content Guidelines:**

```markdown
# Main Topic

Brief introduction to the topic.

## Section 1: Key Points

- Point 1: Explanation
- Point 2: Explanation
- Point 3: Explanation

## Section 2: Details

Detailed information about the topic.

### Subsection

Additional specific information.

## Conclusion

Summary or next steps.
```

**Content Best Practices:**

✅ **DO:**
- Use clear, simple language
- Break content into sections with headings
- Use bullet points for lists
- Keep paragraphs short (2-4 sentences)
- Include specific examples
- Update regularly with current information

❌ **DON'T:**
- Include outdated information
- Use overly technical jargon
- Create duplicate articles
- Leave content incomplete
- Include personal/sensitive data

### Step 3: Save Article

Click **"Save"** to add the article to your knowledge base.

---

## Managing Knowledge Base Articles

### Viewing Articles

**Article List:**

The main Knowledge Base page displays all articles in a table format:

```
ID    TITLE                              EXCERPT                          CREATED AT
6     How to Improve Website Speed       How to Improve Website Speed     17.9.2025 15:41:23
7     SEO Best Practices for 2025        SEO is evolving rapidly...       17.9.2025 15:42:03
8     The Importance of Cybersecurity... The Importance of Cybersecur...  17.9.2025 15:42:16
```

**Sorting and Filtering:**
- Articles display in reverse chronological order (newest first)
- Use table columns to identify articles quickly
- Excerpt provides quick preview of content

### Editing Articles

**To Edit an Article:**

1. Locate the article in the table
2. Click the **Edit icon (✏️)** in the Actions column
3. Modify the title or content as needed
4. Click **"Save"** to update

**When to Edit:**
- Update outdated information
- Improve clarity or accuracy
- Add new details or examples
- Fix errors or typos
- Enhance formatting

!!! tip "Best Practice"
    Regularly review and update articles to ensure your AI Bot has current, accurate information.

### Deleting Articles

**To Delete an Article:**

1. Locate the article in the table
2. Click the **Delete icon (✖)** in the Actions column
3. Confirm deletion when prompted

!!! warning "Deletion is Permanent"
    Deleted articles cannot be recovered. Make sure you want to remove the article before confirming deletion.

**When to Delete:**
- Article contains incorrect information that can't be fixed
- Content is completely outdated
- Duplicate of another article
- No longer relevant to your business

---

## Organizing Your Knowledge Base

### Content Categories

Organize articles by topic for easier management:

**Common Categories:**

```
Product Information
├─ Features and benefits
├─ Pricing and plans
├─ Technical specifications
└─ Product comparisons

Customer Support
├─ Account management
├─ Billing questions
├─ Technical troubleshooting
└─ How-to guides

Company Information
├─ About us
├─ Contact information
├─ Business hours
└─ Policies

Services
├─ Service descriptions
├─ Process explanations
├─ Timeline and delivery
└─ Requirements
```

### Naming Conventions

**Use Consistent Titles:**

✅ **Good Examples:**
- "How to Reset Your Password"
- "What Payment Methods Are Accepted"
- "Shipping Times by Region"
- "Refund Policy Explained"

❌ **Poor Examples:**
- "Password" (too vague)
- "PAYMENT INFO!!!" (inconsistent formatting)
- "shipping" (not descriptive)
- "Policy" (unclear which policy)

---

## Knowledge Base Best Practices

### Content Quality

**Write Clear, Helpful Content:**

**1. Start with the Main Point**
```
✅ Good: "We accept Visa, MasterCard, American Express, and PayPal."
❌ Poor: "In terms of payment options, we have several methods available..."
```

**2. Use Simple Language**
```
✅ Good: "Click the 'Forgot Password' link on the login page."
❌ Poor: "Navigate to the authentication portal and initiate the credential recovery protocol."
```

**3. Be Specific**
```
✅ Good: "Shipping takes 3-5 business days for US orders."
❌ Poor: "Shipping is fast."
```

**4. Include Examples**
```
✅ Good: "Our business hours are Monday-Friday, 9 AM to 5 PM EST. We're closed on major holidays like Christmas and New Year's Day."
❌ Poor: "We're open during normal business hours."
```

### Maintenance Schedule

**Weekly:**
- Review new articles for accuracy
- Check for duplicate content

**Monthly:**
- Update time-sensitive information
- Add new articles based on common questions
- Remove or consolidate outdated articles

**Quarterly:**
- Comprehensive content audit
- Update all articles for accuracy
- Reorganize if needed
- Check for gaps in coverage

---

## How Knowledge Base Works with AI Bot Training

### Integration with Bot Training

Knowledge Base articles automatically become part of your AI Bot's training data:

**Article → Training Flow:**
```
1. Create/Edit Article in Knowledge Base
   ↓
2. Article content added to bot's knowledge
   ↓
3. AI Bot can reference article in responses
   ↓
4. Users get accurate, up-to-date answers
```

### Updating Bot Knowledge

**When you update an article:**
- Changes are reflected in bot training
- Bot responses update with new information
- No manual retraining required

!!! info "Automatic Updates"
    The Knowledge Base syncs with your AI Bot's training data, so updates to articles are automatically available to your bot.

---

## Use Cases

### Customer Support Knowledge Base

**Example Articles:**

```
Title: "How to Reset Your Password"
Content:
To reset your password:
1. Go to the login page
2. Click "Forgot Password"
3. Enter your email address
4. Check your email for reset link
5. Click the link and create new password

Need help? Contact support@company.com

---

Title: "What Are Your Business Hours?"
Content:
We're open:
• Monday-Friday: 9 AM - 5 PM EST
• Saturday: 10 AM - 2 PM EST
• Closed Sundays and major holidays

For urgent issues outside business hours, email support@company.com
```

### Product Information

**Example Articles:**

```
Title: "Basic vs Pro Plan Comparison"
Content:
Basic Plan ($29/month):
• Up to 10 users
• 100 GB storage
• Email support
• Core features

Pro Plan ($79/month):
• Unlimited users
• 1 TB storage
• Priority phone & email support
• Advanced analytics
• Custom integrations
• API access

Start your 14-day free trial of Pro: www.company.com/trial
```

### Policy Information

**Example Articles:**

```
Title: "Refund and Return Policy"
Content:
Our 30-Day Money-Back Guarantee:

Eligible Items:
• Unopened products in original packaging
• Items purchased within last 30 days
• Products with proof of purchase

Return Process:
1. Contact support@company.com
2. Receive return authorization number
3. Ship item with tracking
4. Refund processed within 5-7 business days

Non-Refundable:
• Digital downloads after access
• Customized products
• Sale items marked "Final Sale"
```

---

## Tips for Effective Knowledge Base Management

### Content Creation Tips

**1. Answer Real Questions**
- Base articles on actual customer inquiries
- Address common pain points
- Provide solutions, not just information

**2. Keep It Scannable**
- Use headings and subheadings
- Include bullet points and numbered lists
- Break up long paragraphs
- Highlight key information

**3. Make It Actionable**
- Include step-by-step instructions
- Provide specific examples
- Add links to relevant resources
- Offer contact info for further help

**4. Stay Current**
- Review articles regularly
- Update when policies change
- Remove outdated information
- Add new topics as needed

### Coverage Checklist

Ensure your Knowledge Base covers:

- ☐ Product/service descriptions
- ☐ Pricing and plans
- ☐ How-to guides
- ☐ Account management
- ☐ Billing questions
- ☐ Shipping/delivery info
- ☐ Return/refund policies
- ☐ Contact information
- ☐ Business hours
- ☐ Common troubleshooting issues
- ☐ FAQ topics
- ☐ Company background

---

## Troubleshooting

### Common Issues

**Problem: Article Not Saving**
- **Cause:** Missing required fields (title or content)
- **Solution:** Ensure both title and content are filled in before saving

**Problem: Bot Not Using Article Information**
- **Cause:** Article content too vague or unclear
- **Solution:** Rewrite article with more specific, clear information

**Problem: Duplicate Information**
- **Cause:** Multiple articles covering same topic
- **Solution:** Consolidate into single comprehensive article, delete duplicates

---

## Additional Resources

<div class="grid cards" markdown>

-   :material-school:{ .lg .middle } __Training Guide__

    ---

    Learn more about training your AI Bot

    [:octicons-arrow-right-24: Training Guide](training.md)

-   :material-robot:{ .lg .middle } __Creating AI Bots__

    ---

    Step-by-step bot creation guide

    [:octicons-arrow-right-24: Creating Guide](creating.md)

</div>

---

**Previous:** [← AI Bot Overview](overview.md) | **Next:** [AI Bot Contacts →](contacts.md)

---

**Last Updated:** December 2025
