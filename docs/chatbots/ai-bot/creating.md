# Creating Your First AI Bot

Create a custom AI-powered chatbot for your website in minutes with our step-by-step wizard.

---

## Prerequisites

Before creating your AI Bot, ensure you have:

!!! info "Requirements"
    - ✅ Active iQuivity AI account
    - ✅ Company/product information ready
    - ✅ Content for training (website URLs, documents, or Q&A pairs)
    - ✅ Brand assets (logo, colors) for customization

---

## Accessing AI Bots

### Navigate to AI Bots Dashboard

**Step 1: From Dashboard**
1. Log in to your iQuivity AI account at [iquivity.ai](https://iquivity.ai)
2. From the main dashboard, locate **"AI Bot"** in the left-hand navigation
3. Click on **"AI Bot"** to open the AI Bots dashboard

**Dashboard Overview:**

```
AI Bot Engagement
├── New Agent Messages: 4
├── New AI Messages: 0
└── Total Messages: 57

Active Chatbots (0)
└── [Empty state - no active bots]

Inactive Chatbots (7)
├── iQbot (Created 208 days ago) - Passive
├── iQuivity AIBots (Created 209 days ago) - Passive
├── iQuivity AIBots (Created 209 days ago) - Passive
└── [Additional inactive bots...]
```

---

## Creating a New Chatbot

### Start Creation Process

**Click "+ Add New Chatbot"** (top-right corner of the page)

When you click this button, you'll immediately be taken to the **Configure** page to begin setup.

!!! tip "Quick Setup"
    The wizard consists of 3 main pages: Configure → Customize → Train. Complete each step to create your fully functional AI Bot.

---

## Page 1: Configure

### Company Information

**Company Name** (Required)

```
┌────────────────────────────────────────────────┐
│ Company Name                                   │
│ ┌────────────────────────────────────────────┐ │
│ │ Your Company Name                          │ │
│ └────────────────────────────────────────────┘ │
└────────────────────────────────────────────────┘
```

**Purpose:**
- Identifies your organization in the bot
- Used in internal bot management
- May appear in bot responses
- Helps personalize conversations

**Examples:**
- "Acme Corporation"
- "TechStart Solutions"
- "Global Retail Inc."

---

### Welcome Message

**Welcome Message on Chat Bot** (Required)

```
┌────────────────────────────────────────────────┐
│ Welcome Message on Chat Bot                    │
│ ┌────────────────────────────────────────────┐ │
│ │ Hi! 👋 Welcome to [Company Name].          │ │
│ │ How can I assist you today?               │ │
│ └────────────────────────────────────────────┘ │
└────────────────────────────────────────────────┘
```

**Purpose:**
- First message visitors see when chat opens
- Sets the tone for the conversation
- Creates initial engagement

**Best Practices:**
- ✅ Be friendly and welcoming
- ✅ Keep it concise (1-2 sentences)
- ✅ Use emojis sparingly for personality
- ✅ Indicate you're there to help
- ✅ Use your company/brand name

**Good Examples:**
```
✅ "Hi! I'm here to help with any questions about our products. How can I assist you?"
✅ "Welcome to TechSupport! 👋 What can I help you with today?"
✅ "Hello! Need information about our services? I'm happy to help!"
```

**Avoid:**
```
❌ "Hello." (Too brief)
❌ "Welcome to our website!" (Not helpful)
❌ Long paragraphs explaining everything (Keep it simple)
```

---

### AI Bot Instructions

**Welcome Message on AI Bot** (Required)

```
┌────────────────────────────────────────────────┐
│ AIBot uses a structured set of instruction    │
│ fields that tell the chatbot how to behave,   │
│ what tone to use, what its role is, and how   │
│ to interact with users.                       │
│                                                │
│ ┌────────────────────────────────────────────┐ │
│ │ You are a helpful customer service         │ │
│ │ representative for [Company Name].         │ │
│ │                                            │ │
│ │ - Be friendly and professional             │ │
│ │ - Answer based on knowledge base           │ │
│ │ - If unsure, admit it politely             │ │
│ │ - Keep responses clear and concise         │ │
│ │ - Guide to human support when needed       │ │
│ └────────────────────────────────────────────┘ │
└────────────────────────────────────────────────┘
```

**Purpose:**
- Defines bot's role and personality
- Sets behavioral guidelines
- Establishes response style
- Creates boundaries for bot capabilities

**Instruction Components:**

**1. Role Definition:**
```
"You are a [role] for [company/product]."

Examples:
- "You are a customer support specialist for TechCo."
- "You are a sales assistant for an e-commerce store."
- "You are a virtual tutor for online courses."
```

**2. Behavioral Guidelines:**
```
- Be [adjective] and [adjective]
- Answer questions based on [source]
- Provide [type] of information
- Avoid [behavior]
```

**3. Response Style:**
```
- Keep responses [length]
- Use [tone]
- Format as [style]
- Include [elements]
```

**4. Limitations:**
```
- If you don't know, [action]
- For [topic], [guidance]
- Refer to [resource] when [condition]
```

**Complete Instruction Examples:**

**Customer Support Bot:**
```
You are a friendly customer support representative for Acme Corp.

Guidelines:
- Be helpful, professional, and empathetic
- Answer questions using the knowledge base provided
- If you don't have specific information, say "I don't have that information right now, but I can connect you with a team member"
- Keep responses under 3 sentences when possible
- For billing or account issues, direct users to support@acme.com
- Maintain a positive tone even with frustrated customers
```

**E-commerce Assistant:**
```
You are a shopping assistant for StyleBoutique online store.

Your role:
- Help customers find products
- Provide product information and recommendations
- Answer questions about sizing, materials, and care
- Share shipping and return policies
- For orders and tracking, direct to Order Status page
- Be enthusiastic but not pushy
- Use casual, friendly language
```

**Educational Bot:**
```
You are an academic advisor assistant for University Online Programs.

Responsibilities:
- Provide information about courses and programs
- Answer admission-related questions
- Share application deadlines and requirements
- Explain tuition and financial aid options
- For specific enrollment questions, connect to admissions office
- Be informative and professional
- Encourage prospective students
```

---

### Language Selection

**Choose Bot Languages**

```
┌────────────────────────────────────────────────┐
│ iQuivity allows you to choose which languages  │
│ your AIBot can understand and respond in       │
│ 94 different languages.                        │
│                                                │
│ Primary Language: [English ▼]                 │
│                                                │
│ Additional Languages:                          │
│ ☐ Spanish                                     │
│ ☐ French                                      │
│ ☐ German                                      │
│ ☐ Chinese                                     │
│ ☐ Japanese                                    │
│ ☐ [+ 89 more languages...]                    │
└────────────────────────────────────────────────┘
```

**Purpose:**
- Enable multilingual support
- Auto-detect user language
- Respond in appropriate language
- Expand global reach

**Supported Languages:** 94 languages including:
- English (US, UK, AU)
- Spanish (ES, LA)
- French
- German
- Italian
- Portuguese (BR, PT)
- Chinese (Simplified, Traditional)
- Japanese
- Korean
- Arabic
- Hindi
- Russian
- Dutch
- And 81 more...

**Language Features:**
- Automatic language detection
- User can switch languages mid-conversation
- Knowledge base translated automatically
- Maintains context across language switches

---

### Connect Message

**Platform Connection Message**

```
┌────────────────────────────────────────────────┐
│ Connect Message is the message your AIBot     │
│ sends automatically when it connects to an     │
│ external platform or system, such as:          │
│ Social Media                                   │
│                                                │
│ ┌────────────────────────────────────────────┐ │
│ │ Thanks for reaching out! I'm connected     │ │
│ │ and ready to help. What can I do for you?  │ │
│ └────────────────────────────────────────────┘ │
└────────────────────────────────────────────────┘
```

**Purpose:**
- Confirms successful connection to external platforms
- Acknowledges user initiation from social media
- Sets expectations for the conversation

**Use Cases:**
- Facebook Messenger integration
- Telegram connection
- WhatsApp Business
- Other messaging platforms

**Examples:**
```
✅ "Connected! I'm your virtual assistant. How can I help?"
✅ "Thanks for messaging us! I'm here to answer your questions."
✅ "Hello! I've connected to assist you. What do you need?"
```

---

### Complete Configuration

**Click "Next"** to proceed to the Customize page.

!!! success "Configuration Complete"
    You've set up the core bot behavior. Next, you'll customize the appearance and interaction settings.

---

## Page 2: Customize

### Team Sharing

**Share with Team Members**

```
┌────────────────────────────────────────────────┐
│ This option allows you to give other members  │
│ of your organization access to the AIBot you  │
│ created. When enabled, your bot becomes       │
│ available to everyone on your team inside     │
│ iQuivity.                                      │
│                                                │
│ [ ] Enable Team Sharing                        │
└────────────────────────────────────────────────┘
```

**Purpose:**
- Share bot across organization
- Allow team collaboration
- Enable multiple admins
- Centralized bot management

**When to Enable:**
- Multiple team members need access
- Collaborative bot management
- Shared customer support responsibility
- Team-wide knowledge base updates

**When to Disable:**
- Personal/individual use
- Department-specific bot
- Testing/development bot
- Sensitive information handling

---

### Interaction Type

**Choose Conversation Mode**

```
┌────────────────────────────────────────────────┐
│ Interaction Type setting in iQuivity          │
│ determines how your AIBot engages with users   │
│ and what style of conversation the bot         │
│ follows.                                       │
│                                                │
│ ( ) AI & Live Chat                            │
│ ( ) Only AI                                   │
│ ( ) Only Live Chat                            │
└────────────────────────────────────────────────┘
```

**Option 1: AI & Live Chat (Hybrid)**

```
User → AI Bot → [Optional] Human Agent
```

**Features:**
- AI handles initial conversation
- Users can request human assistance
- "Get More Help" button available
- Seamless handoff to live agents
- Best of both automation and personalization

**Best For:**
- Customer support teams
- Sales inquiries
- Complex product questions
- Quality customer service
- Business with live support team

**Option 2: Only AI**

```
User → AI Bot (Automated)
```

**Features:**
- Fully automated responses
- 24/7 availability
- No human intervention
- Unlimited simultaneous conversations
- Instant responses

**Best For:**
- FAQ handling
- Information distribution
- Simple support queries
- High-volume, low-complexity interactions
- Businesses without live support

**Option 3: Only Live Chat**

```
User → Human Agent (AI Disabled)
```

**Features:**
- Direct connection to human agents
- AI completely disabled
- Traditional live chat experience
- Real-time human support
- Full control over conversations

**Best For:**
- VIP customer support
- Technical troubleshooting
- Sensitive conversations
- High-value sales
- Scenarios requiring human judgment

!!! note "Live Chat Requirements"
    Live chat features require additional configuration and may have separate pricing. Contact sales for enterprise live chat solutions.

---

### Visual Customization

**Chat Widget Appearance**

### Logo Upload

```
┌────────────────────────────────────────────────┐
│ Upload Logo                                    │
│                                                │
│ ┌────────────┐                                │
│ │  [📷]      │  Drag & drop or click          │
│ │  Company   │  to upload                     │
│ │  Logo      │                                │
│ └────────────┘                                │
│                                                │
│ Recommended: 200x200px, PNG/JPG               │
└────────────────────────────────────────────────┘
```

**Logo Guidelines:**
- Format: PNG, JPG, SVG
- Size: 200x200px recommended
- Max file size: 2MB
- Transparent background preferred
- High resolution for clarity

---

### Avatar Upload

```
┌────────────────────────────────────────────────┐
│ Upload Avatar                                  │
│                                                │
│ ┌────────────┐                                │
│ │  [👤]      │  Drag & drop or click          │
│ │  Bot       │  to upload                     │
│ │  Avatar    │                                │
│ └────────────┘                                │
│                                                │
│ Recommended: 128x128px, PNG/JPG               │
└────────────────────────────────────────────────┘
```

**Avatar Guidelines:**
- Format: PNG, JPG
- Size: 128x128px recommended
- Circular crop automatically applied
- Represents bot in chat interface

---

### Color Scheme

**Header Background Style**

```
┌────────────────────────────────────────────────┐
│ You can choose the background style for the   │
│ chat header. Currently, Solid Color is        │
│ selected, with a color picker available.      │
│                                                │
│ Header Background:                             │
│ ( ) Solid Color  [🎨 #4F46E5]                │
│ ( ) Gradient                                   │
│                                                │
│ Primary Color:    [🎨 #4F46E5]               │
│ Secondary Color:  [🎨 #3B82F6]               │
│ Text Color:       [🎨 #FFFFFF]               │
│ Background Color: [🎨 #F9FAFB]               │
└────────────────────────────────────────────────┘
```

**Color Customization:**

**Primary Color:**
- Main brand color
- Chat bubble background
- Header background
- Action buttons

**Secondary Color:**
- Accent elements
- Links
- Secondary buttons
- Hover states

**Text Color:**
- Button text
- Header text
- Ensure good contrast

**Background Color:**
- Chat window background
- Message area
- Light, neutral recommended

---

### Feature Toggles

**Optional Chat Features**

```
┌────────────────────────────────────────────────┐
│ When you turn these options on, we allow you   │
│ to receive:                                    │
│                                                │
│ [ ] Email Collect                             │
│     Enable collection of user emails          │
│                                                │
│ [ ] Contact Us                                │
│     Show "Contact Us" option in chat          │
│                                                │
│ [ ] Enable Emoji                              │
│     Allow emojis in chat interactions         │
│                                                │
│ [ ] Show Logo                                 │
│     Display logo in chat widget header        │
│                                                │
│ [ ] Show Date and Time                        │
│     Display timestamps for messages           │
│                                                │
│ [ ] Transparent Trigger                       │
│     Make chat trigger button transparent      │
└────────────────────────────────────────────────┘
```

**Feature Descriptions:**

**Email Collect:**
- Prompt users for email before/during chat
- Build contact list
- Follow up via email
- Lead generation tool

**Contact Us:**
- Add "Contact Us" button in chat
- Link to contact form or email
- Escalation option for users
- Collect inquiries

**Enable Emoji:**
- Allow emoji in user messages
- Enable emoji in bot responses
- Makes chat more friendly
- Enhances expression

**Show Logo:**
- Display company logo in header
- Reinforces branding
- Professional appearance
- Brand recognition

**Show Date and Time:**
- Timestamp on each message
- Conversation history context
- Useful for support records
- Professional communication

**Transparent Trigger:**
- Chat button with transparent background
- Minimalist design
- Blends with website
- Less intrusive

---

### Widget Position & Size

**Trigger Avatar Size**

```
┌────────────────────────────────────────────────┐
│ Adjust the size of the chat trigger           │
│ button/avatar.                                 │
│                                                │
│ Trigger Size: [60]px                          │
│ ├───────────●──────┤                          │
│ 40px              100px                        │
└────────────────────────────────────────────────┘
```

**Size Recommendations:**
- **Small (40-50px):** Subtle, minimalist sites
- **Medium (60-70px):** Standard, most websites
- **Large (80-100px):** Prominent, high-traffic sites

---

**Position on Page**

```
┌────────────────────────────────────────────────┐
│ Choose which side of the page the chat widget │
│ trigger appears.                               │
│                                                │
│ Horizontal Position:                           │
│ ( ) Left                                      │
│ (•) Right   [Currently Selected]              │
│                                                │
│ Vertical Position:                             │
│ ( ) Top-Left                                  │
│ ( ) Top-Right                                 │
│ (•) Bottom-Left                               │
│ ( ) Bottom-Right  [Currently Selected]        │
└────────────────────────────────────────────────┘
```

**Position Options:**

**Horizontal:**
- **Right:** Most common, matches user reading pattern
- **Left:** Alternative for specific layouts

**Vertical:**
- **Bottom-Right:** Standard position, most familiar
- **Bottom-Left:** Alternative positioning
- **Top-Right:** For sticky header designs
- **Top-Left:** Rare, specific use cases

**Best Practices:**
- Bottom-right is standard and expected
- Avoid blocking important content
- Consider mobile responsiveness
- Test on different screen sizes
- Ensure easy access without obstruction

---

### Font Selection

```
┌────────────────────────────────────────────────┐
│ Chat Font:                                     │
│ [Roboto ▼]                                    │
│                                                │
│ Available Fonts:                               │
│ - Roboto (Default)                             │
│ - Open Sans                                    │
│ - Lato                                         │
│ - Montserrat                                   │
│ - Poppins                                      │
│ - Inter                                        │
│ + Custom font upload                           │
└────────────────────────────────────────────────┘
```

---

### Complete Customization

**Click "Next"** to proceed to the Training page.

!!! success "Customization Complete"
    Your bot now has a unique look and feel that matches your brand. Next, you'll train it with your knowledge base.

---

## Page 3: Training

**Training Page Overview:**

```
┌────────────────────────────────────────────────┐
│ What Training page means and why it matters    │
│                                                │
│ When you build a custom bot on iQuivity, you're│
│ not just relying on a generic AI—you will train│
│ the bot on your own content/data. That way,    │
│ when a user asks a question, the bot can answer│
│ with accurate, company-specific information.   │
│                                                │
│ The "Training page" is where you feed content  │
│ into the bot: upload documents, import website │
│ pages, define QA pairs, etc., and thereby build│
│ what the bot "knows."                          │
│                                                │
│ A well-trained bot makes your chatbot much more│
│ reliable, reduces "I don't know" responses, and│
│ ensures answers match your business information│
│ so training is arguably the most important step│
│ after bot creation.                            │
└────────────────────────────────────────────────┘
```

**Training will be covered in detail in the next section.**

[:octicons-arrow-right-24: Training & Knowledge](training.md)

---

## Review & Deploy

### Final Steps

After completing all three pages (Configure, Customize, Train), you're ready to deploy:

**1. Review Configuration**
```
✅ Company name and welcome message set
✅ Bot instructions defined
✅ Languages selected
✅ Connect message configured
```

**2. Review Customization**
```
✅ Team sharing configured
✅ Interaction type selected
✅ Logo and avatar uploaded
✅ Colors and branding applied
✅ Features enabled/disabled
✅ Position and size set
```

**3. Review Training**
```
✅ Knowledge sources added
✅ Documents uploaded
✅ Q&A pairs defined
✅ Bot tested and verified
```

**Click "Next"** to proceed to deployment and get your embed code.

---

## Bot Actions & Management

### Bot Dashboard Actions

From the AI Bots dashboard, each bot has action menu (⋮):

```
Bot Actions Menu:
├── Edit
├── Customize
├── Train
├── Test & Embed
├── Channel
├── Activate
└── Delete
```

**Edit:**
- Modify configure settings
- Update welcome messages
- Change instructions
- Adjust languages

**Customize:**
- Update appearance
- Change colors and branding
- Modify features
- Adjust positioning

**Train:**
- Add/remove knowledge sources
- Upload new documents
- Update Q&A pairs
- Refresh training data

**Test & Embed:**
- Preview bot functionality
- Test conversations
- Get embed code
- Copy widget script

**Channel:**
- Configure deployment channels
- Set up social media integration
- Manage platform connections
- Configure webhooks

**Activate:**
- Toggle bot active/inactive status
- Enable for production use
- Publish to website

**Delete:**
- Permanently remove bot
- Cannot be undone
- Frees up bot slot in plan

---

## Bot Status

### Active vs Passive Status

**Active Chatbots:**
- Currently deployed and running
- Receiving and responding to messages
- Visible on website/platforms
- Consuming API credits

**Passive/Inactive Chatbots:**
- Created but not deployed
- Not receiving messages
- Not visible to users
- No credit consumption
- Can be activated anytime

**Status Indicator:**
```
iQbot
Created 208 days ago
[Passive]
```

---

## Testing Your Bot

### Before Going Live

**Use Test & Embed Feature:**

1. Click action menu (⋮) on your bot
2. Select "Test & Embed"
3. Opens preview window
4. Test various scenarios:
   - ☐ Welcome message displays
   - ☐ Bot responds accurately
   - ☐ Trained content accessible
   - ☐ Unknown questions handled gracefully
   - ☐ Human handoff works (if enabled)
   - ☐ Appearance looks correct
   - ☐ Mobile responsive

---

## Best Practices

### Creating Effective Bots

**Configuration Tips:**

✅ **Clear Company Identity**
- Use recognizable company name
- Be consistent with branding
- Match website voice and tone

✅ **Welcoming Messages**
- Keep welcome message under 2 sentences
- Be friendly and approachable
- Set clear expectations

✅ **Specific Instructions**
- Define clear boundaries
- Specify what bot can/cannot do
- Include escalation procedures
- Set response style guidelines

✅ **Language Support**
- Enable languages your customers speak
- Test in each language
- Ensure knowledge base translates well

**Customization Tips:**

✅ **Brand Consistency**
- Match website colors exactly
- Use company logo and fonts
- Maintain visual identity

✅ **User Experience**
- Standard bottom-right position
- Appropriate trigger size
- Enable helpful features (emoji, timestamps)
- Don't block important content

✅ **Mobile Optimization**
- Test on various devices
- Ensure touch-friendly size
- Check responsive behavior
- Verify readability

**Training Tips:**

✅ **Comprehensive Knowledge**
- Cover common questions thoroughly
- Include product/service details
- Add policy information
- Update regularly

✅ **Quality Over Quantity**
- Accurate information essential
- Well-organized content
- Clear, concise answers
- Avoid contradictions

---

## Troubleshooting

### Common Issues

**Bot Not Responding:**
- **Cause:** Not trained yet, no knowledge added
- **Solution:** Complete training step, add content sources

**Incorrect Responses:**
- **Cause:** Insufficient or incorrect training data
- **Solution:** Review and improve knowledge base

**Appearance Issues:**
- **Cause:** Color conflicts, size problems
- **Solution:** Adjust colors for contrast, test sizes

**Deployment Problems:**
- **Cause:** Incorrect embed code, script conflicts
- **Solution:** Follow deployment guide exactly, check for JS conflicts

---

## Next Steps

<div class="grid cards" markdown>

-   :material-school:{ .lg .middle } __Train Your Bot__

    ---

    Add knowledge from multiple sources

    [:octicons-arrow-right-24: Training Guide](training.md)

-   :material-palette:{ .lg .middle } __Advanced Customization__

    ---

    Fine-tune appearance and behavior

    [:octicons-arrow-right-24: Customization Details](customization.md)

-   :material-rocket-launch:{ .lg .middle } __Deploy to Website__

    ---

    Get embed code and go live

    [:octicons-arrow-right-24: Deployment Guide](deployment.md)

</div>

---

**Previous:** [← Overview](overview.md) | **Next:** [Training →](training.md)

---

**Last Updated:** December 2025
