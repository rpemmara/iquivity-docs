# IQ Bot - Overview

## What is IQ Bot?

**IQ Bot** is an AI-powered mini-site that consolidates multiple business functions within a single URL-accessible interface, fundamentally transforming how users interact with business services by eliminating navigation between separate systems.

!!! success "Unified Engagement Platform"
    IQ Bot presents websites, calendars, videos, documents, video calls, and AI chat in one seamless interface - accessed through a single URL or QR code.

---

## The Problem IQ Bot Solves

### Fragmented Digital Experience

**Current Challenge:**

Existing web engagement systems lead to static content and fragmented user experiences. Users must navigate multiple disparate systems for different actions:

```
Traditional Approach (High Friction):
├─ Visit website for information
├─ Navigate to separate chat system
├─ Open calendar tool for scheduling
├─ Switch to video conferencing platform
├─ Access document portal separately
└─ Use different system for purchasing
```

**Impact of Fragmentation:**
- Creates friction at every step
- Multiple abandonment opportunities
- Major cause of funnel drop-off
- Lost conversions and revenue
- Poor user experience

**IQ Bot Solution:**

```
IQ Bot Approach (Zero Friction):
┌────────────────────────────────────────┐
│  Single URL: iquivity.net/iqbot/name   │
├────────────────────────────────────────┤
│  ┌──────────────────────────────────┐  │
│  │ [Welcome] [Chat] [Calendar]      │  │
│  │ [Video] [Docs] [Buy Now]         │  │
│  ├──────────────────────────────────┤  │
│  │                                  │  │
│  │  All functions in one place      │  │
│  │  Unified interface               │  │
│  │  Shared context                  │  │
│  │  AI assistant always available   │  │
│  │                                  │  │
│  └──────────────────────────────────┘  │
└────────────────────────────────────────┘
```

**Result:**
- Enhanced customer engagement
- Reduced friction and abandonment
- Higher conversion rates
- Increased revenues
- Superior user experience

---

## How IQ Bot Works

### Technology Architecture

**Unified Interface System:**

When users access an IQ Bot URL, the system opens a unified interface containing multiple selectable tabs. Each tab provides distinct functionality while maintaining shared context and user session information across all interactions.

```
┌─────────────────────────────────────────────┐
│  IQ Bot: https://test.iquivity.net/iqbot/  │
│          [your-bot-name]                    │
├─────────────────────────────────────────────┤
│                                             │
│  Tab Navigation:                            │
│  ┌─────┬──────┬──────────┬───────┬──────┐  │
│  │ 🏠  │ 💬   │ 📅       │ 🎥    │ 🛒   │  │
│  │Welcome│Chat│Calendar  │Video  │Buy   │  │
│  └─────┴──────┴──────────┴───────┴──────┘  │
│                                             │
│  ┌─────────────────────────────────────┐   │
│  │                                     │   │
│  │   Active Tab Content:               │   │
│  │   - Website pages (linked/embedded) │   │
│  │   - Calendar scheduling             │   │
│  │   - Video content or calls          │   │
│  │   - Documents and PDFs              │   │
│  │   - Custom forms and pages          │   │
│  │                                     │   │
│  └─────────────────────────────────────┘   │
│                                             │
│  🤖 AI Chat available anytime              │
└─────────────────────────────────────────────┘
```

**Key Characteristics:**
- **Dynamic Generation** - Tabs are dynamically generated for each session, unlike static webpages
- **Shared Context** - User session information maintained across all tabs
- **Instant Updates** - Tabs can be added, edited, or removed with immediate effect
- **Easy Activation** - Can be activated/deactivated instantly

---

## Core Components

### 1. AI Chatbot Foundation

**Intelligent Assistant:**

An AI chatbot trained on business data underlies the IQ Bot, available at any time to answer questions.

**AI Chatbot Features:**
- Trained on websites, documents, raw text, and Q&A
- Answers questions based on your business data
- Human agent transfer capability (SMS alert)
- Available across all tabs

**Training Process:**

```
Data Sources → Chunking → Vector Embeddings → Vector Database
                                                    ↓
User Question → Retrieval → Context + Question → AI Model → Answer
```

**Technology:**
1. **Data Chunking** - Breaking content into manageable pieces
2. **Vector Embeddings** - Converting text to AI-understandable format
3. **Vector Database** - Storing indexed knowledge
4. **Retrieval** - Finding relevant information
5. **AI Generation** - Creating accurate answers

### 2. Tab System

**Flexible Content Tabs:**

IQ Bot supports multiple tab types for different content:

| Tab Type | Purpose | Examples |
|----------|---------|----------|
| **Welcome** | Introduction and overview | Landing page, company info |
| **Chat** | AI chatbot interface | Customer support, Q&A |
| **Calendar Link** | Appointment scheduling | Booking, consultation scheduling |
| **Video Call** | Video conference integration | Meetings, consultations |
| **Videos (YouTube)** | Video content display | Product demos, tutorials |
| **Websites** | Website pages (link/embed) | Product pages, information |
| **Buy Now** | Purchase links and pages | E-commerce, checkout |
| **Reviews** | Customer testimonials | Social proof, feedback |
| **Docs** | Document access | PDFs, guides, manuals |
| **Custom Tab** | Custom pages and forms | Forms, workflows, custom content |

**Tab Configuration:**
- **Linked Content** - Opens external URLs
- **Embedded Content** - Displays content within IQ Bot interface
- **Custom Pages** - Create forms and workflows
- **Instant Updates** - Add, edit, or delete tabs anytime

### 3. URL and QR Code System

**Access Methods:**

Each IQ Bot gets a unique URL and QR code for easy sharing:

```
┌─────────────────────────────────────────┐
│  IQ Bot Access                          │
├─────────────────────────────────────────┤
│                                         │
│  URL: https://test.iquivity.net/iqbot/ │
│       adbot1                            │
│                                         │
│  QR Code: [QR CODE IMAGE]              │
│           ▄▄▄▄▄▄▄   ▄ ▄   ▄▄▄▄▄▄▄      │
│           █     █  ██▄█   █     █      │
│           █ ███ █ ▄▀█▄▀   █ ███ █      │
│           █ ███ █ ▀ █ ▄   █ ███ █      │
│           █     █ ███ █   █     █      │
│           ▀▀▀▀▀▀▀ ▀ ▀ ▀   ▀▀▀▀▀▀▀      │
│                                         │
│  [Download QR Code]                     │
│                                         │
└─────────────────────────────────────────┘
```

**Usage Scenarios:**
- Business cards
- Marketing materials
- Email signatures
- Social media profiles
- Print advertising
- Event materials
- Digital displays

### 4. Analytics Dashboard

**Comprehensive Usage Analytics:**

IQ Bot includes a detailed analytics dashboard that presents data about tab usage:

**Analytics Views:**
- **Daily** - 24-hour activity
- **Weekly** - 7-day trends (default)
- **Monthly** - 30-day overview
- **Custom** - Date range selection

**Key Metrics:**

```
┌────────────────────────────────────────────┐
│  IQ Bot Analytics Dashboard                │
├────────────────────────────────────────────┤
│                                            │
│  📊 Total Tab Views              4  0.00%  │
│  ⏱️  Average Time Spent on Tab   0  0.00%  │
│  📅 Total Time Spent per Day     0  0.00%  │
│  🖱️  Daily Tab Clicks            0  0.00%  │
│                                            │
│  Engagement Charts:                        │
│  ├─ IQ Bot Clicks (timeline)              │
│  ├─ IQ Bot Interactions (timeline)        │
│  ├─ Popular Tabs (ranking)                │
│  └─ Time Spent in IQ Bot Tabs (minutes)   │
│                                            │
│  Geographic Data:                          │
│  ├─ IQ Bot Geo-Analytics (map)            │
│  └─ Top vs Bottom Locations               │
│                                            │
│  Platform Analytics:                       │
│  ├─ Platform Breakdown                    │
│  └─ Share Platform (UTM)                  │
│                                            │
└────────────────────────────────────────────┘
```

**Analytics Capabilities:**
- Track which tabs are most popular
- Monitor time spent on each tab
- View click patterns and engagement
- Geographic distribution of visitors
- Platform and device breakdown
- Traffic source tracking (UTM)

---

## Key Advantages

### 🎯 Unified User Experience

**Single Access Point:**
- One URL for all business functions
- No navigation between systems
- Shared user context across tabs
- Seamless experience

### ⚡ Instant Updates

**Dynamic Content Management:**
```
Unlike static websites:
├─ Add new tabs instantly
├─ Edit existing tabs anytime
├─ Delete outdated tabs immediately
├─ Activate/deactivate entire IQ Bot easily
└─ Changes take effect immediately
```

### 🤖 AI-Powered Assistance

**Always-Available Intelligence:**
- Trained on your business data
- Answers questions across all tabs
- Human handoff when needed
- Context-aware responses

### 📊 Data-Driven Insights

**Comprehensive Analytics:**
- Understand user behavior
- Identify popular content
- Track engagement metrics
- Optimize based on data

### 📱 Multi-Platform Access

**Available Everywhere:**
- Direct URL access
- QR code scanning
- Mobile-responsive interface
- Desktop and tablet optimized

---

## IQ Bot vs AI Bot Comparison

Understanding the difference between IQ Bot and AI Bot:

| Aspect | IQ Bot | AI Bot |
|--------|---------|---------|
| **Primary Purpose** | Unified mini-site with multiple functions | Website chatbot widget |
| **Interface** | Multi-tab interface with various content types | Single chat interface |
| **Content Types** | Websites, calendars, videos, docs, forms, chat | Chat conversations only |
| **Access Method** | Dedicated URL + QR code | Embedded widget on your site |
| **AI Component** | Underlying chatbot available across tabs | Primary and only feature |
| **URL Sharing** | ✅ Unique URL for each IQ Bot | ❌ No standalone URL |
| **QR Code** | ✅ Automatic generation | ❌ Not applicable |
| **Tab System** | ✅ Multiple configurable tabs | ❌ N/A |
| **Analytics** | Comprehensive tab usage analytics | Chat conversation analytics |
| **Use Case** | Centralized business hub | Customer support chat |
| **Best For** | Consolidating multiple touchpoints | Adding chat to existing website |
| **Activation** | Can be enabled/disabled easily | Always embedded when installed |
| **Custom Forms** | ✅ Create workflows and forms | ❌ Limited to chat |

**When to Use Each:**

**Use IQ Bot When:**
- You need to consolidate multiple business functions
- You want a shareable URL for campaigns
- You need QR codes for print/physical materials
- You want analytics on content engagement
- You're creating a landing page alternative
- You want flexibility to add/remove content quickly

**Use AI Bot When:**
- You want to add chat to an existing website
- Your primary need is customer support
- You want embedded chat on specific pages
- You need traditional chatbot functionality

---

## Use Cases

### 1. Event Management

**Conference or Event IQ Bot:**

```
┌─────────────────────────────────────┐
│  Event IQ Bot                       │
├─────────────────────────────────────┤
│  Tabs:                              │
│  ├─ Welcome: Event overview         │
│  ├─ Schedule: Agenda and calendar   │
│  ├─ Speakers: Video profiles        │
│  ├─ Register: Registration form     │
│  ├─ Venue: Location and directions  │
│  ├─ Chat: AI assistant for Q&A      │
│  └─ Feedback: Post-event survey     │
└─────────────────────────────────────┘
```

**Distribution:**
- QR codes on event posters
- URL in email invitations
- Shared on social media
- Printed on conference badges

### 2. Product Launch

**New Product IQ Bot:**

```
Tabs:
├─ Welcome: Product introduction
├─ Features: Detailed specifications
├─ Demo Video: Product walkthrough
├─ Pricing: Buy Now integration
├─ Reviews: Customer testimonials
├─ Docs: User manual and guides
├─ Support: Chat with product experts
└─ Calendar: Schedule consultation
```

**Benefits:**
- All product information in one place
- Easy sharing via QR code
- Track which features get attention
- Capture leads through forms

### 3. Service Provider Hub

**Consultant or Agency IQ Bot:**

```
Tabs:
├─ Welcome: About and services
├─ Portfolio: Case studies website
├─ Calendar: Book consultation
├─ Video Call: Join meeting room
├─ Proposals: Document access
├─ Pricing: Service packages
├─ Chat: Instant questions
└─ Custom Form: Project inquiry
```

**Use Cases:**
- Email signature link
- Business card QR code
- LinkedIn profile
- Proposal follow-ups

### 4. Restaurant or Venue

**Hospitality IQ Bot:**

```
Tabs:
├─ Welcome: Restaurant intro
├─ Menu: Food and drinks (PDF)
├─ Reserve: Booking calendar
├─ Gallery: Photo/video tour
├─ Reviews: Customer feedback
├─ Order: Online ordering system
├─ Location: Map and directions
└─ Chat: Questions and support
```

**Deployment:**
- QR codes on table tents
- Window displays
- Business cards
- Google Business Profile

### 5. Real Estate Listing

**Property Showcase IQ Bot:**

```
Tabs:
├─ Welcome: Property overview
├─ Photos: Image gallery
├─ Video Tour: Walkthrough video
├─ Floor Plans: PDF documents
├─ Schedule: Book showing
├─ Calculator: Mortgage form
├─ Agent Chat: Questions
└─ Apply: Application form
```

**Marketing:**
- Yard sign QR codes
- Listing websites
- Email campaigns
- Print advertising

---

## IQ Bot Management

### Dashboard Overview

**IQ Bots Dashboard:**

```
┌────────────────────────────────────────────────┐
│  IQ Bots                                       │
│  View and manage IQbots                        │
│                                [+ Add New Bot] │
├────────────────────────────────────────────────┤
│                                                │
│  IQ Bot Engagement                             │
│  ├─ Count Per Month:           0               │
│  ├─ Active IQBots Per Month:   0               │
│  └─ Show Total Count:          6               │
│                                                │
│  Active IQBots (0)                             │
│  [Search Active IQ bots]                       │
│  [Empty state illustration]                    │
│                                                │
│  Inactive IQBots (2)                           │
│  [Search Inactive IQ bots]                     │
│  ┌──────────────┐  ┌──────────────┐           │
│  │ Adbot1       │  │ Trading Bot  │           │
│  │ Created 107  │  │ Created 107  │           │
│  │ days ago     │  │ days ago     │           │
│  │              │  │              │           │
│  │ URL + QR     │  │ URL + QR     │           │
│  │ [Download]   │  │ [Download]   │           │
│  └──────────────┘  └──────────────┘           │
│                                                │
│  Deleted IQBots (0)                            │
│  [Empty state illustration]                    │
│                                                │
└────────────────────────────────────────────────┘
```

### Bot Actions Menu

**Available Actions:**

From the IQ Bots dashboard, each bot has an action menu (⋮):

```
Bot Actions:
├── Edit        - Modify bot settings (name, AI Bot association)
├── Analytics   - View detailed usage analytics
├── Share       - Access URL and QR code
├── Activate    - Make bot live/inactive (toggle)
└── Delete      - Move to deleted (30-day retention)
```

### Bot States

**Active vs Inactive:**

- **Active IQBots** - Live and accessible via URL
- **Inactive IQBots** - Created but not activated, URL displays inactive state
- **Deleted IQBots** - Soft deleted, 30-day recovery window

**Status Management:**
```
Create → Inactive (default) → Activate → Active
                                ↓
                             Deactivate → Inactive
                                ↓
                             Delete → Deleted (30 days) → Permanent Deletion
                                ↓
                             Restore → Inactive
```

---

## Creating an IQ Bot

### Creation Process

**Simple Setup Steps:**

1. **Associate AI Bot** - Select which AI chatbot to use for the IQ Bot
2. **Configure General Settings** - Name, description, tab orientation
3. **Create Tabs** - Add and configure tabs with content
4. **Customize Appearance** - Logo, colors, fonts (optional)
5. **Review and Activate** - Test and make live

**Quick Example:**

```yaml
IQ Bot Configuration:
  ai_bot: "Customer Support Bot"
  name: "Adbot1"
  description: "Welcome message for visitors"
  tab_orientation: "Horizontal"  # or Vertical
  tab_style: "Rounded Top"

  tabs:
    - title: "Buy Now"
      description: "50% discount"
      type: "Link"
      url: "https://yoursite.com/products"
      button_text: "Shop Now"

    - title: "Welcome"
      description: "Hello"
      type: "Embed"
      content: "Welcome message content"
```

**Result:**
- URL: `https://test.iquivity.net/iqbot/adbot1`
- QR Code: Automatically generated
- Status: Inactive (activate when ready)

---

## Getting Started

Ready to create your first IQ Bot?

<div class="grid cards" markdown>

-   :material-rocket-launch:{ .lg .middle } __Create IQ Bot__

    ---

    Step-by-step guide to creating your first IQ Bot

    [:octicons-arrow-right-24: Getting Started Guide](getting-started.md)

-   :material-chart-line:{ .lg .middle } __Analytics__

    ---

    Understanding IQ Bot analytics and metrics

    [:octicons-arrow-right-24: Analytics Guide](../ai-bot/analytics.md)

</div>

---

## Benefits Summary

### For Businesses

**Operational Benefits:**
- ✅ Consolidate multiple systems into one
- ✅ Reduce friction in customer journey
- ✅ Increase conversion rates
- ✅ Improve user engagement
- ✅ Gain actionable insights from analytics
- ✅ Easy to update and maintain
- ✅ Cost-effective compared to multiple tools

**Marketing Benefits:**
- ✅ Shareable URLs for campaigns
- ✅ QR codes for print materials
- ✅ Track engagement metrics
- ✅ A/B test different content
- ✅ Retarget based on tab views

### For Users

**User Benefits:**
- ✅ Everything in one place
- ✅ No navigation between systems
- ✅ Fast and responsive interface
- ✅ AI assistant always available
- ✅ Mobile-friendly experience
- ✅ Easy to bookmark and return

---

## Success Metrics

**Typical IQ Bot Performance:**

```
┌────────────────────────────────────────┐
│ Average IQ Bot Impact                  │
├────────────────────────────────────────┤
│                                        │
│ User Engagement:        +45%           │
│ Conversion Rate:        +32%           │
│ Bounce Rate:           -28%            │
│ Time on Site:          +67%            │
│ Share Rate:            +89%            │
│ Mobile Usage:          +56%            │
│                                        │
└────────────────────────────────────────┘
```

---

!!! tip "Quick Start"
    Create your first IQ Bot in under 10 minutes. No technical skills required!

    [:octicons-arrow-right-24: Get Started Now](getting-started.md)

**Next:** [Getting Started with IQ Bot →](getting-started.md)
