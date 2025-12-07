# Deploying Your AI Bot

Learn how to deploy your AI Bot across multiple channels - website, Facebook Messenger, Telegram, WhatsApp, and configure Human Agent handoff.

---

## Deployment Options

Your AI Bot can be deployed across multiple platforms simultaneously:

<div class="grid cards" markdown>

-   :material-web:{ .lg .middle } __Website Widget__

    ---

    Embed on any website with simple JavaScript code

    **Setup Time:** 5 minutes

-   :fontawesome-brands-facebook-messenger:{ .lg .middle } __Facebook Messenger__

    ---

    Connect to your Facebook Page

    **Setup Time:** 15 minutes

-   :fontawesome-brands-telegram:{ .lg .middle } __Telegram__

    ---

    Deploy as a Telegram bot

    **Setup Time:** 10 minutes

-   :fontawesome-brands-whatsapp:{ .lg .middle } __WhatsApp Business__

    ---

    Connect via Twilio integration

    **Setup Time:** 20 minutes

-   :material-account-voice:{ .lg .middle } __Human Agent__

    ---

    Enable live chat handoff to human agents

    **Setup Time:** 15 minutes

</div>

---

## Website Deployment

### Overview

The website widget is the most common deployment method. It adds a chat bubble to your website that visitors can click to start conversations.

### Step 1: Get Embed Code

**From AI Bot Dashboard:**

1. Navigate to your AI Bot
2. Click **"Deploy"** or **"Embed"**
3. Select **"Website Widget"**
4. Copy the embed code

**Embed Code Example:**
```html
<script>
  window.iQuivityAI = {
    botId: "your-bot-id-here",
    apiKey: "your-api-key"
  };
</script>
<script src="https://app.iquivity.ai/embed/chatbot.js" defer></script>
```

### Step 2: Add to Your Website

**For Most Websites:**

Add the code before the closing `</body>` tag:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Your Website</title>
</head>
<body>
  <!-- Your website content -->

  <!-- AI Bot Embed Code - Add before </body> -->
  <script>
    window.iQuivityAI = {
      botId: "your-bot-id-here",
      apiKey: "your-api-key"
    };
  </script>
  <script src="https://app.iquivity.ai/embed/chatbot.js" defer></script>
</body>
</html>
```

**For WordPress:**

1. Go to **Appearance** → **Theme Editor**
2. Open **footer.php**
3. Add code before `</body>`
4. Save changes

Or use a plugin like "Insert Headers and Footers"

**For Shopify:**

1. Go to **Online Store** → **Themes**
2. Click **Actions** → **Edit Code**
3. Open **theme.liquid**
4. Add code before `</body>`
5. Save

**For Wix:**

1. Go to **Settings** → **Custom Code**
2. Click **+ Add Custom Code**
3. Paste embed code
4. Set to load on **All Pages**
5. Place in **Body - end**

### Step 3: Configure Widget Settings

**Appearance Settings:**

| Setting | Options | Description |
|---------|---------|-------------|
| **Position** | Bottom Right / Bottom Left | Chat bubble location |
| **Theme** | Light / Dark / Auto | Color scheme |
| **Size** | Small / Medium / Large | Widget size |
| **Z-Index** | Number (default: 999999) | Layer priority |

**Behavior Settings:**

| Setting | Options | Description |
|---------|---------|-------------|
| **Auto-Open** | On / Off | Open automatically |
| **Auto-Open Delay** | Seconds (0-60) | Delay before opening |
| **Welcome Bubble** | On / Off | Show notification bubble |
| **Sound** | On / Off | Notification sound |

**Advanced Settings:**

```javascript
window.iQuivityAI = {
  botId: "your-bot-id",
  apiKey: "your-api-key",

  // Appearance
  position: "bottom-right", // or "bottom-left"
  theme: "auto", // "light", "dark", or "auto"
  primaryColor: "#4F46E5",

  // Behavior
  autoOpen: false,
  autoOpenDelay: 5, // seconds
  showWelcomeBubble: true,
  welcomeBubbleDelay: 3,

  // User Information (optional)
  user: {
    name: "John Doe",
    email: "john@example.com",
    customData: {
      plan: "premium"
    }
  }
};
```

### Step 4: Test the Widget

**Testing Checklist:**

- ☐ Chat bubble appears in correct position
- ☐ Widget opens when clicked
- ☐ Welcome message displays
- ☐ Bot responds to test questions
- ☐ Colors match your branding
- ☐ Mobile responsiveness works
- ☐ Widget doesn't interfere with site elements

**Browser Testing:**
- Chrome (desktop & mobile)
- Safari (desktop & mobile)
- Firefox
- Edge

### Troubleshooting Website Deployment

**Widget Not Appearing:**
- Check if embed code is before `</body>`
- Verify bot ID and API key are correct
- Check browser console for errors
- Ensure no ad blockers are active

**Widget Conflicts with Site Elements:**
- Adjust z-index value
- Change widget position
- Reduce widget size
- Modify auto-open behavior

**Slow Loading:**
- Use `defer` attribute in script tag
- Check website's overall performance
- Consider lazy loading widget

---

## Facebook Messenger Integration

### Overview

Connect your AI Bot to Facebook Messenger so customers can interact via Facebook.

### Prerequisites

**Before starting, you need:**

- ☐ Facebook Page (business page)
- ☐ Facebook Developer Account
- ☐ Admin access to the Facebook Page
- ☐ AI Bot configured and trained

### Step 1: Create Facebook App

**1. Go to Facebook Developers**
- Visit: https://developers.facebook.com
- Log in with your Facebook account

**2. Create New App**
- Click **"My Apps"** → **"Create App"**
- Select **"Business"** as app type
- Click **"Continue"**

**3. Configure App Details**
```
App Name: [Your Company] Chatbot
App Contact Email: your-email@company.com
Business Account: [Select your business]
```

Click **"Create App"**

**4. Add Messenger Product**
- In dashboard, find **"Messenger"**
- Click **"Set Up"**

### Step 2: Generate Page Access Token

**1. Select Your Page**
- Under **"Access Tokens"**
- Select your Facebook Page
- Click **"Generate Token"**

**2. Grant Permissions**
Required permissions:
- `pages_messaging`
- `pages_manage_metadata`
- `pages_read_engagement`

**3. Copy Token**
```
EAAxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

!!! warning "Keep Token Secret"
    Never share your Page Access Token publicly. Store it securely.

### Step 3: Configure Webhook

**1. In iQuivity AI Dashboard**
- Go to your AI Bot
- Click **"Integrations"** → **"Facebook Messenger"**
- Copy the **Callback URL** and **Verify Token**

**Callback URL:**
```
https://app.iquivity.ai/webhook/facebook/your-bot-id
```

**Verify Token:**
```
your-verify-token-here
```

**2. In Facebook App Dashboard**
- Go to **Messenger** → **Settings**
- Under **Webhooks**, click **"Add Callback URL"**

**3. Enter Webhook Details**
```
Callback URL: [Paste from iQuivity]
Verify Token: [Paste from iQuivity]
```

Click **"Verify and Save"**

**4. Subscribe to Events**

Select these webhook fields:
- ☑ `messages`
- ☑ `messaging_postbacks`
- ☑ `message_deliveries`
- ☑ `message_reads`

Click **"Subscribe"**

### Step 4: Connect Page to Bot

**1. In iQuivity AI Dashboard**

Enter your Facebook Page Access Token:
```
Page Access Token: EAAxxxxxxx...
Page ID: [Your Facebook Page ID]
```

**2. Test Connection**

Click **"Test Connection"**

✅ Success: "Connected to Facebook Page: [Your Page Name]"

### Step 5: Test Facebook Messenger

**1. Find Your Page on Facebook**
- Go to your Facebook Page
- Click **"Send Message"**

**2. Send Test Message**
```
User: Hello
Bot: [Welcome message]

User: What are your hours?
Bot: [Response from training data]
```

### Step 6: Submit for Review (Optional)

**For Public Use:**

Facebook requires app review for public bots:

1. Go to **App Review** in Facebook App dashboard
2. Request permissions for **pages_messaging**
3. Provide app details and use case
4. Submit for review (1-2 weeks processing)

!!! info "Testing vs Production"
    During development, your bot works with admins/testers only. After review, it's public.

### Facebook Messenger Best Practices

**DO:**
- ✅ Respond within 24 hours to messages
- ✅ Use Facebook's Get Started button
- ✅ Provide clear menu options
- ✅ Test with multiple users before launch
- ✅ Monitor response times

**DON'T:**
- ❌ Send spam or unsolicited messages
- ❌ Violate Facebook's platform policies
- ❌ Collect sensitive info via Messenger
- ❌ Use for political campaigns without approval

### Troubleshooting Facebook Integration

**Problem: Webhook Verification Failed**
- **Cause:** Incorrect verify token
- **Solution:** Ensure verify token matches exactly (case-sensitive)

**Problem: Bot Not Responding**
- **Cause:** Webhook not subscribed to page
- **Solution:** In Facebook App, subscribe webhook to your page

**Problem: "This app is in development mode"**
- **Cause:** App not approved for public use
- **Solution:** Submit for app review or add testers manually

---

## Telegram Integration

### Overview

Deploy your AI Bot as a Telegram bot accessible to Telegram users worldwide.

### Prerequisites

- ☐ Telegram account
- ☐ AI Bot configured and trained

### Step 1: Create Telegram Bot

**1. Open Telegram**
- Search for **@BotFather**
- Start a conversation

**2. Create New Bot**

Send command:
```
/newbot
```

**3. Name Your Bot**

BotFather will ask:
```
Alright, a new bot. How are we going to call it?
```

Enter your bot name:
```
My Company Support Bot
```

**4. Choose Username**
```
Now choose a username for your bot. It must end in `bot`.
```

Enter username (must be unique):
```
mycompany_support_bot
```

**5. Get Bot Token**

BotFather responds with:
```
Done! Your bot is ready.
Token: 123456789:ABCdefGHIjklMNOpqrsTUVwxyz
```

!!! warning "Keep Token Secret"
    Store your bot token securely. Don't share it publicly.

### Step 2: Configure in iQuivity AI

**1. Go to AI Bot Dashboard**
- Select your AI Bot
- Click **"Integrations"** → **"Telegram"**

**2. Enter Bot Token**
```
Bot Token: 123456789:ABCdefGHIjklMNOpqrsTUVwxyz
```

Click **"Connect"**

**3. Verify Connection**

✅ Success: "Connected to Telegram Bot: @mycompany_support_bot"

### Step 3: Configure Bot Settings

**In BotFather, configure:**

**Set Description:**
```
/setdescription @mycompany_support_bot
```
Enter description users see before starting:
```
Welcome! I'm here to help you with your questions about our products and services.
```

**Set About Text:**
```
/setabouttext @mycompany_support_bot
```
Enter about text (shown in bot profile):
```
Customer support bot for MyCompany
```

**Set Profile Photo:**
```
/setuserpic @mycompany_support_bot
```
Upload your logo or bot avatar

**Set Commands:**
```
/setcommands @mycompany_support_bot
```
Enter commands:
```
start - Start conversation
help - Get help
contact - Contact support
reset - Start new conversation
```

### Step 4: Test Your Telegram Bot

**1. Find Your Bot**
- Search for `@mycompany_support_bot` in Telegram
- Click **"Start"**

**2. Test Interactions**
```
User: /start
Bot: [Welcome message]

User: What are your hours?
Bot: [Response from training]

User: /help
Bot: [Help information]
```

### Telegram Bot Features

**Available Commands:**

Create custom commands in iQuivity dashboard:

| Command | Function | Example |
|---------|----------|---------|
| `/start` | Begin conversation | Default welcome |
| `/help` | Show help | List available commands |
| `/contact` | Contact human | Escalate to support |
| `/reset` | Reset conversation | Clear chat history |

**Interactive Buttons:**

Add reply keyboards for common actions:
```
[View Products] [Check Status]
[Contact Support] [FAQ]
```

**Rich Media Support:**
- Send images, PDFs, links
- Receive file uploads from users
- Display formatted messages

### Telegram Best Practices

**DO:**
- ✅ Use clear, concise messages
- ✅ Implement useful commands
- ✅ Add interactive buttons
- ✅ Respond quickly (Telegram users expect speed)
- ✅ Use formatting (bold, italics, lists)

**DON'T:**
- ❌ Send unsolicited messages
- ❌ Spam users with notifications
- ❌ Violate Telegram's terms of service
- ❌ Request sensitive info without encryption

### Troubleshooting Telegram Integration

**Problem: Bot Not Responding**
- **Cause:** Token not configured correctly
- **Solution:** Re-enter token in iQuivity dashboard

**Problem: Commands Not Working**
- **Cause:** Commands not registered with BotFather
- **Solution:** Use `/setcommands` to configure

**Problem: "Bot was blocked by the user"**
- **Cause:** User blocked your bot
- **Solution:** User must unblock to receive messages

---

## WhatsApp Integration

### Overview

Connect your AI Bot to WhatsApp Business using Twilio integration.

### Prerequisites

**Required:**
- ☐ Twilio account (free trial available)
- ☐ WhatsApp Business account
- ☐ Verified phone number
- ☐ AI Bot configured and trained

### Step 1: Set Up Twilio Account

**1. Create Twilio Account**
- Go to: https://www.twilio.com/try-twilio
- Sign up for free account
- Verify your email and phone

**2. Get Account Credentials**

From Twilio Console:
```
Account SID: ACxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
Auth Token: your_auth_token_here
```

### Step 2: Configure WhatsApp Sandbox (Testing)

**For Testing (Free):**

**1. In Twilio Console**
- Navigate to **Messaging** → **Try it out** → **Send a WhatsApp message**

**2. Join Sandbox**
- Send WhatsApp message to Twilio's sandbox number
- Follow instructions to join

**3. Get Sandbox Details**
```
Phone Number: +1 415 xxx xxxx
Sandbox Join Code: join [unique-code]
```

### Step 3: Get Production WhatsApp Number

**For Production (Paid):**

**1. Request WhatsApp Business Account**
- In Twilio: **Messaging** → **WhatsApp** → **Senders**
- Click **"Request Access"**

**2. Provide Business Information**
```
Business Name: [Your Company]
Business Website: https://yourcompany.com
Business Description: [What you do]
Phone Number: [Your WhatsApp Business number]
```

**3. Submit for Approval**
- Twilio review: 1-3 business days
- WhatsApp approval: 2-7 days

### Step 4: Configure Webhook in Twilio

**1. In iQuivity AI Dashboard**
- Go to your AI Bot
- Click **"Integrations"** → **"WhatsApp"**
- Copy the **Webhook URL**

```
https://app.iquivity.ai/webhook/whatsapp/your-bot-id
```

**2. In Twilio Console**
- Go to **Messaging** → **Settings** → **WhatsApp Sandbox Settings**
- Under **"When a message comes in"**

**3. Configure Webhook**
```
URL: [Paste iQuivity webhook URL]
HTTP Method: POST
```

Click **"Save"**

### Step 5: Connect to iQuivity AI

**1. In iQuivity Dashboard**

Enter Twilio credentials:
```
Account SID: ACxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
Auth Token: your_auth_token
WhatsApp Number: +1415xxxxxxx
```

**2. Test Connection**

Click **"Connect WhatsApp"**

✅ Success: "WhatsApp connected successfully"

### Step 6: Test WhatsApp Bot

**For Sandbox Testing:**

1. Send message to sandbox number with join code:
```
join unique-code
```

2. Send test questions:
```
User: Hello
Bot: [Welcome message]

User: What are your hours?
Bot: [Response]
```

**For Production:**

Users can directly message your WhatsApp Business number.

### WhatsApp Message Templates

**For Outbound Messages:**

WhatsApp requires pre-approved templates for business-initiated messages.

**1. Create Template in Twilio**
- Go to **Messaging** → **WhatsApp** → **Templates**
- Click **"Create Template"**

**2. Template Example**
```
Name: order_confirmation
Category: Order Update
Language: English

Content:
Hello {{1}}, your order #{{2}} has been confirmed!
We'll notify you when it ships.
```

**3. Submit for Approval**
- WhatsApp reviews templates (24-48 hours)

### WhatsApp Integration Features

**Supported:**
- ✅ Text messages
- ✅ Media messages (images, PDFs)
- ✅ Location sharing
- ✅ Quick replies
- ✅ Message templates

**Limitations:**
- ❌ Can't initiate conversation without template (24hr window)
- ❌ Rate limits apply
- ❌ Some emoji may not display correctly

### WhatsApp Best Practices

**DO:**
- ✅ Get user consent before messaging
- ✅ Use templates for proactive messages
- ✅ Respond within 24-hour window
- ✅ Provide opt-out option
- ✅ Follow WhatsApp Business Policy

**DON'T:**
- ❌ Send spam or promotional content
- ❌ Share user data with third parties
- ❌ Use for customer acquisition without consent
- ❌ Violate WhatsApp Commerce Policy

### Pricing

**Twilio WhatsApp Pricing:**
- Inbound messages: $0.005 per message
- Outbound messages: $0.005 - $0.04 (varies by country)
- Free trial credits available

### Troubleshooting WhatsApp Integration

**Problem: Webhook Not Receiving Messages**
- **Cause:** Incorrect webhook URL
- **Solution:** Verify URL is correct and uses HTTPS

**Problem: "Unable to Send Message"**
- **Cause:** Outside 24-hour response window
- **Solution:** Use approved message template

**Problem: Template Rejected**
- **Cause:** Violates WhatsApp policy
- **Solution:** Review policy and revise template

---

## Human Agent Integration

### Overview

Enable live chat handoff so visitors can seamlessly escalate from AI Bot to human agents through the CRM Inbox.

### Prerequisites

**Required:**
- ☐ AI Bot with "AI + Live Chat" interaction type enabled
- ☐ Human agents ready to respond
- ☐ Access to CRM Inbox

### Step 1: Enable Human Agent Feature

**1. Configure Your AI Bot**
- Go to **AI Bot** → **Settings**
- Under **Interaction Type**, select **"AI + Live Chat"**
- Configure handoff button text (e.g., "Get More Help", "Talk to Human")
- Set availability hours for human agents
- Save configuration

**2. Bot Interaction Settings**

The AI Bot will automatically provide a handoff option to users when:
- User requests to speak with a human agent
- AI Bot cannot answer a question
- User clicks the "Get More Help" button

### Step 2: Access CRM Inbox

**1. Navigate to CRM Inbox**
- Go to main menu: **CRM Inbox** or **Live Chat**
- View all incoming conversations from AI Bots

**2. Inbox Overview**

The CRM Inbox shows:
- **All conversations** from all channels (Website, Facebook, Telegram, WhatsApp)
- **Conversation status**: All, Open, Closed
- **Filter by channel**: All Channel, LiveChat, Telegram, WhatsApp, Messenger
- **Filter by agent**: All, AI Agent, Human Agent
- **Sort by**: Newest, oldest, etc.

### Step 3: Managing Conversations

**1. View Conversation Details**

Click on any conversation to see:
- **User Information**: Name, channel, contact details
- **Conversation History**: Full chat transcript
- **Contact Details**: ID, Status (New/Open/Closed), Created date, Updated date, Country, IP Address
- **Conversation ID**: Unique identifier for each chat

**2. Available Actions**

For each conversation, you can:
- **Reply to messages**: Send responses directly in the chat
- **View conversation history**: See full AI and human agent interactions
- **Delete conversation**: Remove conversation from inbox
- **Export conversation**: Download chat transcript
- **Change status**: Mark as Open or Closed

### Step 4: How Handoff Works

**User Journey:**

```
1. User starts chat with AI Bot
   ↓
2. AI Bot handles initial questions
   ↓
3. User clicks "Get More Help" button or requests human
   ↓
4. Conversation appears in CRM Inbox
   ↓
5. Human agent views and responds to conversation
   ↓
6. Human agent continues conversation until resolved
   ↓
7. Agent marks conversation as Closed when complete
```

**CRM Inbox View:**

The inbox displays conversations with:
- **Contact name/ID**: Anonymous User or identified contact
- **Channel indicator**: @livechat, @telegram, @messenger
- **Last message preview**: Recent message text
- **Timestamp**: When last message was received
- **Status indicator**: New, Open, or Closed

### Step 5: Responding to Conversations

**1. Select a Conversation**
- Click on any conversation in the inbox
- View conversation history and user details
- Review what the AI Bot has already discussed

**2. Send a Response**
- Type your message in the message field
- Click **Send** or press Enter
- Message appears in the conversation thread

**3. Best Practices**

**DO:**
- ✅ Review AI conversation history before responding
- ✅ Introduce yourself as a human agent
- ✅ Be friendly and professional
- ✅ Provide clear, helpful responses
- ✅ Mark conversations as Closed when resolved

**DON'T:**
- ❌ Keep users waiting without acknowledgment
- ❌ Ignore conversation context from AI Bot
- ❌ Give contradictory information from what AI provided
- ❌ Leave conversations unresolved

### Step 6: Conversation Management

**Filtering Conversations:**

Use inbox filters to organize conversations:
- **By Status**: View All, Open, or Closed conversations
- **By Channel**: Filter by LiveChat, Telegram, WhatsApp, Messenger
- **By Agent Type**: See AI Agent or Human Agent conversations
- **By Date**: Sort by Newest or oldest first

**Conversation Actions:**

From the conversation menu (⋮), you can:
- **Delete**: Remove conversation from inbox
- **Export Conversation**: Download chat transcript for records

**Tracking Conversation Details:**

Each conversation displays:
- **ID**: Unique conversation identifier
- **Status**: New, Open, or Closed
- **Created**: When conversation started
- **Updated**: Last message timestamp
- **Country**: User's country code
- **IP Address**: User's IP (for security/tracking)

### Troubleshooting Human Agent

**Problem: Not Seeing New Conversations**
- **Cause:** Filter settings or page not refreshed
- **Solution:** Refresh the CRM Inbox page, check filter settings (ensure "All" is selected)

**Problem: Cannot Reply to Conversation**
- **Cause:** Conversation may be closed or user disconnected
- **Solution:** Check conversation status, reopen if needed

**Problem: Missing Conversation History**
- **Cause:** Conversation was deleted or system issue
- **Solution:** Check "All" filter to ensure conversation wasn't closed, contact support if data is missing

---

## Multi-Channel Deployment

### Deploy Everywhere

Your AI Bot can run on **all channels simultaneously**:

```
              ┌─────────────┐
              │   AI Bot    │
              │  (Central)  │
              └──────┬──────┘
                     │
        ┌────────────┼────────────┐
        │            │            │
   [Website]   [Facebook]   [Telegram]
        │            │            │
        └────────────┼────────────┘
                     │
              [WhatsApp]
                     │
              [Human Agent]
```

### Benefits of Multi-Channel:

- ✅ Meet customers where they are
- ✅ Consistent experience across platforms
- ✅ Centralized training and management
- ✅ Centralized CRM inbox for all channels
- ✅ Single knowledge base

---

## Security & Compliance

### Data Protection

**SSL/TLS Encryption:**
- All data transmitted over HTTPS
- End-to-end encryption available

**Data Storage:**
- Conversations stored securely
- GDPR compliant
- Data retention policies configurable

**Privacy Controls:**
- User data anonymization
- Opt-out options
- Data deletion requests

### Compliance

**Supported Standards:**
- GDPR (EU)
- CCPA (California)
- HIPAA (Healthcare) - Enterprise only
- SOC 2 Type II

---

## Deployment Checklist

### Pre-Launch Checklist

Before going live, verify:

**AI Bot Configuration:**
- ☐ Bot fully trained with comprehensive knowledge
- ☐ Welcome message configured
- ☐ Operating hours set (if applicable)
- ☐ Branding and colors match company style
- ☐ Email collection configured (if needed)

**Channel Setup:**
- ☐ Website embed code added and tested
- ☐ Facebook Messenger connected (if using)
- ☐ Telegram bot configured (if using)
- ☐ WhatsApp integration tested (if using)
- ☐ Human Agent dashboard configured (if using)

**Testing:**
- ☐ Test conversations on all channels
- ☐ Verify mobile responsiveness
- ☐ Check cross-browser compatibility
- ☐ Test human handoff (if enabled)

**Documentation:**
- ☐ Internal team trained on agent dashboard
- ☐ Response templates created
- ☐ Escalation procedures documented
- ☐ Maintenance schedule established

---

## Monitoring & Maintenance

### Post-Deployment Monitoring

**Daily:**
- Check for unanswered questions
- Monitor response accuracy
- Review agent performance (if applicable)

**Weekly:**
- Review CRM inbox for common questions
- Add new Q&A pairs based on questions
- Update training data as needed

**Monthly:**
- Comprehensive performance review
- Training data audit
- Update seasonal content

---

---

**Previous:** [← Training](training.md) | **Up:** [AI Bot Overview](overview.md)

---

**Last Updated:** December 2025
