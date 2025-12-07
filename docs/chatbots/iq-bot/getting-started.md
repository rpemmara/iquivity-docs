# Getting Started with IQ Bot

Welcome to IQ Bot! This guide will walk you through creating and deploying your first AI-powered mini-site that consolidates multiple business functions into one unified interface.

## Prerequisites

Before you begin, ensure you have:

- [x] **Active iQuivity Account** - Sign up at [iquivity.ai](https://iquivity.ai)
- [x] **AI Bot Created** - You'll need an AI Bot to associate with your IQ Bot
- [x] **Content Ready** - Websites, calendars, videos, or documents you want to include
- [x] **Appropriate Permissions** - Required to create and configure IQ Bots

!!! tip "Create AI Bot First"
    IQ Bot requires an underlying AI chatbot. If you haven't created one yet, see the [AI Bot Creation Guide](../ai-bot/creating.md).

---

## Quick Start Overview

Creating an IQ Bot involves five simple steps:

```
Step 1: Access IQ Bot Dashboard
        ↓
Step 2: Configure General Settings
        ↓
Step 3: Create and Configure Tabs
        ↓
Step 4: Review and Test
        ↓
Step 5: Activate and Share
```

---

## Step 1: Access IQ Bot Dashboard

### Navigate to IQ Bots

From your iQuivity dashboard:

```
Dashboard → Chatbots → IQ Bots → + Add New Bot
```

**IQ Bots Dashboard Overview:**

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
│  Inactive IQBots (2)                           │
│  Deleted IQBots (0)                            │
│                                                │
└────────────────────────────────────────────────┘
```

**Dashboard Sections:**
- **IQ Bot Engagement** - Overview metrics
- **Active IQBots** - Live and accessible mini-sites
- **Inactive IQBots** - Created but not yet activated
- **Deleted IQBots** - Recently deleted (30-day recovery)

!!! note "Initial State"
    New IQ Bots start as "Inactive" by default. You'll activate them after configuration and testing.

---

## Step 2: Configure General Settings

### Page: General

When you click "+ Add New Bot", you'll see the General configuration page:

```
┌─────────────────────────────────────────────────┐
│  General                                        │
│  Create and configure a chatbot that interacts │
│  with your users, ensuring it delivers         │
│  accurate information.                          │
├─────────────────────────────────────────────────┤
│                                                 │
│  AI Bot *                                       │
│  ┌────────────────────────────────────────┐    │
│  │ No AI Bot                         ▼    │    │
│  └────────────────────────────────────────┘    │
│                                                 │
│  Name *                                         │
│  ┌────────────────────────────────────────┐    │
│  │ Adbot1                                 │    │
│  └────────────────────────────────────────┘    │
│                                                 │
│  Description                                    │
│  ┌────────────────────────────────────────┐    │
│  │ Enter welcome message                  │    │
│  │                                        │    │
│  │                                        │    │
│  └────────────────────────────────────────┘    │
│                                                 │
│  Tab Orientation *                              │
│  ┌───────────┐  ┌───────────┐                  │
│  │ ─────     │  │     │     │                  │
│  │ Horizontal│  │ Vertical  │                  │
│  └───────────┘  └───────────┘                  │
│  [✓ Horizontal]                                 │
│                                                 │
│  Note: Vertical scrollbar not appearing in     │
│  preview/responsive mode                        │
│                                                 │
│  Tab Style                                      │
│  ┌────────────────────────────────────────┐    │
│  │ Rounded Top                       ▼    │    │
│  └────────────────────────────────────────┘    │
│                                                 │
│  Upload Logo                                    │
│  [Choose File] No file chosen                  │
│  [Preview of uploaded logo]                    │
│                                                 │
│  Do you want to share this IQ Bot with your    │
│  team?                                         │
│  ○ No   ○ Yes                                  │
│                                                 │
└─────────────────────────────────────────────────┘
```

### Configuration Fields

#### AI Bot (Required)

**Select AI Chatbot:**

Choose which AI Bot will power the chat functionality in your IQ Bot.

```yaml
Field: AI Bot
Type: Dropdown
Required: Yes
Options: List of your created AI Bots
Default: "No AI Bot"
```

**Important:**
- You must have an AI Bot created first
- The AI Bot handles all chat interactions
- Trained on your business data
- Available across all tabs

!!! warning "No AI Bot Available?"
    If you see "No AI Bot" in the dropdown, you need to create an AI Bot first. Visit [AI Bot Creation Guide](../ai-bot/creating.md).

#### Name (Required)

**IQ Bot Name:**

```yaml
Field: Name
Type: Text input
Required: Yes
Max length: 50 characters
Example: "Adbot1", "ProductHub", "EventCenter"
```

**Naming Guidelines:**
- Short and memorable
- No special characters or spaces
- Used in URL: `https://test.iquivity.net/iqbot/[name]`
- Cannot be changed after creation

**URL Format:**
```
https://test.iquivity.net/iqbot/adbot1
                                  └─ Your bot name here
```

#### Description (Optional)

**Welcome Message:**

```yaml
Field: Description
Type: Text area
Required: No
Purpose: Internal reference or welcome message
Max length: 500 characters
```

**Usage:**
- Describe the purpose of your IQ Bot
- Internal notes for team members
- Welcome message for users

#### Tab Orientation (Required)

**Choose Layout:**

**Horizontal (Recommended):**
```
┌──────────────────────────────────────┐
│ [Welcome] [Chat] [Calendar] [Video]  │
│ ────────────────────────────────────│
│                                      │
│        Tab Content Here              │
│                                      │
└──────────────────────────────────────┘
```

**Vertical:**
```
┌─────────┬────────────────────────────┐
│ Welcome │                            │
│ Chat    │                            │
│ Calendar│     Tab Content Here       │
│ Video   │                            │
│ Docs    │                            │
└─────────┴────────────────────────────┘
```

!!! note "Vertical Mode Note"
    Vertical scrollbar may not appear in preview/responsive mode. This is a known display behavior.

**Best Practices:**
- **Horizontal** - Better for 3-6 tabs, desktop/tablet users
- **Vertical** - Better for 6+ tabs, mobile-first approach

#### Tab Style

**Visual Appearance:**

```yaml
Field: Tab Style
Type: Dropdown
Default: "Rounded Top"
Options:
  - Rounded Top    # Rounded corners on top
  - Square         # Square tabs
  - Rounded All    # Fully rounded tabs
  - Minimal        # Simple underline style
```

**Preview:**
```
Rounded Top:  ┌────┐ ┌────┐ ┌────┐
              │Tab1│ │Tab2│ │Tab3│
              └────┴─┴────┴─┴────┴─

Square:       ┌────┬─┬────┬─┬────┐
              │Tab1│ │Tab2│ │Tab3│
              └────┴─┴────┴─┴────┴─

Rounded All:  ╭────╮ ╭────╮ ╭────╮
              │Tab1│ │Tab2│ │Tab3│
              └────┴─┴────┴─┴────┴─

Minimal:       Tab1   Tab2   Tab3
              ─────  ──────  ─────
```

#### Upload Logo

**Brand Your IQ Bot:**

```yaml
Field: Upload Logo
Type: File upload
Accepted: PNG, JPG, SVG
Max size: 5MB
Recommended: 200x200px, transparent background
Position: Displays in tab header/navigation
```

**Logo Guidelines:**
- Square or horizontal format
- Transparent background preferred
- High resolution for retina displays
- Matches your brand identity

#### Team Sharing

**Share with Organization:**

```yaml
Field: Do you want to share this IQ Bot with your team?
Type: Radio buttons
Options:
  - No  (Default)
  - Yes
```

**Sharing Options:**
- **No** - Only you can edit and manage
- **Yes** - All team members can access and manage

!!! tip "Team Collaboration"
    Enable sharing if multiple team members need to update tabs or review analytics.

---

## Step 3: Create and Configure Tabs

### Page: Tabs

After completing General settings, you'll navigate to the Tabs configuration page:

```
┌─────────────────────────────────────────────────┐
│  Tabs                                           │
│  Create and configure a chatbot that interacts │
│  with your users, ensuring it delivers         │
│  accurate information.                          │
├─────────────────────────────────────────────────┤
│                                                 │
│  Select Tab                                     │
│  ┌────────────────────────────────────────┐    │
│  │ -- Select Tab --                  ▼    │    │
│  └────────────────────────────────────────┘    │
│                                                 │
│  ┌═══════════════════════════════════════┐    │
│  ║  ⋮⋮  Buy Now                       ▼  ×║    │
│  ╠───────────────────────────────────────╣    │
│  ║  Title                                 ║    │
│  ║  ┌────────────────────────────────┐   ║    │
│  ║  │ Buy Now                        │   ║    │
│  ║  └────────────────────────────────┘   ║    │
│  ║                                        ║    │
│  ║  Description                           ║    │
│  ║  ┌────────────────────────────────┐   ║    │
│  ║  │ 50% discount                   │   ║    │
│  ║  │                                │   ║    │
│  ║  └────────────────────────────────┘   ║    │
│  ║                                        ║    │
│  ║  Select Content Type                   ║    │
│  ║  ┌────────────────────────────────┐   ║    │
│  ║  │ Link                      ▼    │   ║    │
│  ║  └────────────────────────────────┘   ║    │
│  ║                                        ║    │
│  ║  Link Configuration                    ║    │
│  ║  Enter Link URL *                      ║    │
│  ║  ┌────────────────────────────────┐   ║    │
│  ║  │ <a href="undefined">[object    │   ║    │
│  ║  │  Object]</a>                   │   ║    │
│  ║  └────────────────────────────────┘   ║    │
│  ║  At least one valid link URL is    ║    │
│  ║  required.                             ║    │
│  ║                                        ║    │
│  ║  ┌────────────────────────────────┐   ║    │
│  ║  │ Button Text               [+]  │   ║    │
│  ║  └────────────────────────────────┘   ║    │
│  ║  Button text is required.              ║    │
│  ║                                        ║    │
│  ║  ┌────────────────────────────────┐   ║    │
│  ║  │ Description                    │   ║    │
│  ║  └────────────────────────────────┘   ║    │
│  ║                                        ║    │
│  └═══════════════════════════════════════┘    │
│                                                 │
│  [+ Add Tab]                                   │
│                                                 │
└─────────────────────────────────────────────────┘
```

### Select Tab Dropdown

**Available Tab Types:**

Click the "-- Select Tab --" dropdown to see all available tab types:

```
┌────────────────────────────────┐
│ ✓ -- Select Tab --             │
├────────────────────────────────┤
│   Welcome ✓                    │
│   Chat                         │
│   Calendar Link                │
│   Video Call                   │
│   Videos (Youtube Links)       │
│   Websites                     │
│   Buy Now ✓                    │
│   Reviews                      │
│   Docs                         │
│   Custom Tab                   │
└────────────────────────────────┘
```

**Tab Types Explained:**

| Tab Type | Purpose | Content Options |
|----------|---------|-----------------|
| **Welcome** ✓ | Landing/introduction page | Text, images, embedded content |
| **Chat** | AI chatbot interface | Automatically uses selected AI Bot |
| **Calendar Link** | Appointment scheduling | Calendly, Google Calendar, etc. |
| **Video Call** | Video conference link | Zoom, Meet, Teams links |
| **Videos (YouTube)** | Video content | YouTube embed links |
| **Websites** | Website pages | Link or embed external sites |
| **Buy Now** | Purchase/product pages | E-commerce links or embedded shop |
| **Reviews** | Testimonials/feedback | Review platforms or custom content |
| **Docs** | Documents and PDFs | Document viewers, download links |
| **Custom Tab** | Any custom content | Forms, workflows, custom HTML |

✓ = Commonly selected tabs

!!! tip "Tab Selection Strategy"
    Start with 3-5 essential tabs. You can easily add more later based on analytics data showing user needs.

### Tab Configuration

Each tab has common configuration fields:

#### Tab Header

```
⋮⋮  Buy Now                                    ▼  ×
└─┘  └────┘                                    └┘ └┘
 │      │                                       │  │
 │      └─ Tab title (changeable)              │  │
 └─ Drag handle (reorder tabs)                 │  │
                           Collapse/expand tab ─┘  │
                                       Delete tab ─┘
```

**Tab Controls:**
- **⋮⋮ Drag Handle** - Click and drag to reorder tabs
- **▼ Collapse** - Expand/collapse tab configuration
- **× Delete** - Remove tab from IQ Bot

#### Title (Required)

```yaml
Field: Title
Type: Text input
Required: Yes
Max length: 30 characters
Display: Shows on tab navigation
Example: "Buy Now", "Welcome", "Contact"
```

**Title Guidelines:**
- Short and clear (2-3 words max)
- Action-oriented when possible
- Matches user expectations
- Consistent capitalization

#### Description (Optional)

```yaml
Field: Description
Type: Text area
Required: No
Max length: 200 characters
Purpose: Additional context for tab content
Example: "50% discount on all products"
```

**Usage:**
- Brief description of tab content
- Call-to-action text
- Special offers or highlights
- Internal notes

#### Select Content Type

**Link vs Embed:**

```yaml
Field: Select Content Type
Type: Dropdown
Options:
  - Link   # Opens in new tab/window
  - Embed  # Displays within IQ Bot interface
```

**Link Content Type:**
```
User clicks tab → Opens URL in new window
Best for: External websites, checkout pages, video calls
```

**Embed Content Type:**
```
User clicks tab → Shows content within IQ Bot
Best for: Videos, calendars, documents, forms
```

!!! warning "Embed Limitations"
    Some websites prevent embedding (X-Frame-Options). If embed doesn't work, use Link instead.

### Link Configuration

When "Link" is selected as content type:

```
┌─────────────────────────────────────────┐
│  Link Configuration                     │
├─────────────────────────────────────────┤
│                                         │
│  Enter Link URL *                       │
│  ┌────────────────────────────────┐    │
│  │ https://yoursite.com/products  │    │
│  └────────────────────────────────┘    │
│  At least one valid link URL is         │
│  required.                              │
│                                         │
│  ┌────────────────────────────────┐    │
│  │ Button Text               [+]  │    │
│  └────────────────────────────────┘    │
│  Button text is required.               │
│                                         │
│  ┌────────────────────────────────┐    │
│  │ Description (optional)         │    │
│  └────────────────────────────────┘    │
│                                         │
└─────────────────────────────────────────┘
```

#### Enter Link URL (Required)

**URL Field:**

```yaml
Field: Enter Link URL
Type: Text input or rich text editor
Required: Yes (at least one valid URL)
Format: Full URL with https://
Validation: Must be valid URL format
```

**URL Examples:**
```
Product page:     https://yoursite.com/products
Calendar:         https://calendly.com/username
Video call:       https://zoom.us/j/meeting-id
YouTube:          https://youtube.com/watch?v=video-id
Document:         https://drive.google.com/file/d/file-id
Buy Now:          https://yoursite.com/checkout
```

**Multiple URLs:**

You can add multiple buttons with the [+] button:

```
┌─────────────────────────────────────┐
│  Button 1:                          │
│  URL: https://site.com/product-a    │
│  Text: "View Product A"             │
│                                     │
│  Button 2:                      [+] │
│  URL: https://site.com/product-b    │
│  Text: "View Product B"             │
│                                     │
│  Button 3:                      [+] │
│  URL: https://site.com/compare      │
│  Text: "Compare Products"           │
└─────────────────────────────────────┘
```

!!! tip "Multiple Buttons"
    Use multiple buttons to give users options (e.g., "Basic Plan", "Pro Plan", "Enterprise").

#### Button Text (Required)

```yaml
Field: Button Text
Type: Text input
Required: Yes (for each URL)
Max length: 50 characters
Purpose: Text displayed on clickable button
```

**Button Text Examples:**
```
Tab Type          | Button Text Examples
──────────────────|───────────────────────────────
Buy Now          | "Shop Now", "Buy Product", "Get Started"
Calendar         | "Book Appointment", "Schedule Call"
Video Call       | "Join Meeting", "Start Video Chat"
Website          | "Visit Site", "Learn More", "View Page"
Documents        | "Download PDF", "View Guide", "Read More"
```

**Best Practices:**
- Action verbs (Shop, Book, Join, Download)
- Clear and specific
- Creates urgency or value
- Mobile-friendly length

#### Description (Optional)

```yaml
Field: Description
Type: Text area
Required: No
Purpose: Additional context for button
Display: Shown near button
```

### Embed Configuration

When "Embed" is selected:

```
┌─────────────────────────────────────────┐
│  Embed Configuration                    │
├─────────────────────────────────────────┤
│                                         │
│  Embed Code or URL *                    │
│  ┌────────────────────────────────┐    │
│  │ <iframe src="..."              │    │
│  │   width="100%"                 │    │
│  │   height="600">                │    │
│  │ </iframe>                      │    │
│  └────────────────────────────────┘    │
│                                         │
│  OR                                     │
│                                         │
│  ┌────────────────────────────────┐    │
│  │ https://youtube.com/embed/...  │    │
│  └────────────────────────────────┘    │
│                                         │
└─────────────────────────────────────────┘
```

**Embed Options:**
1. **iFrame Code** - Paste full iframe HTML
2. **Embed URL** - Direct URL to embeddable content
3. **YouTube** - Video embed links
4. **Calendar** - Calendly/Google Calendar widgets
5. **Documents** - Google Docs, PDFs

**Common Embed Examples:**

**YouTube Video:**
```html
<iframe width="560" height="315"
  src="https://www.youtube.com/embed/VIDEO_ID"
  frameborder="0" allowfullscreen>
</iframe>
```

**Calendly:**
```html
<div class="calendly-inline-widget"
  data-url="https://calendly.com/username/30min"
  style="min-width:320px;height:630px;">
</div>
```

**Google Doc:**
```html
<iframe
  src="https://docs.google.com/document/d/DOC_ID/preview"
  width="100%" height="600">
</iframe>
```

### Tab Examples

#### Example 1: Welcome Tab

```yaml
Tab Configuration:
  type: "Welcome"
  title: "Welcome"
  description: "Learn about our services"
  content_type: "Embed"
  content: |
    <div style="padding: 20px;">
      <h2>Welcome to Our Service</h2>
      <p>Explore our tabs to learn more!</p>
    </div>
```

#### Example 2: Buy Now Tab

```yaml
Tab Configuration:
  type: "Buy Now"
  title: "Buy Now"
  description: "50% discount today!"
  content_type: "Link"
  links:
    - url: "https://shop.example.com/products"
      button_text: "Shop Now"
      description: "Browse all products"
    - url: "https://shop.example.com/deals"
      button_text: "View Deals"
      description: "Limited time offers"
```

#### Example 3: Calendar Tab

```yaml
Tab Configuration:
  type: "Calendar Link"
  title: "Schedule"
  description: "Book your free consultation"
  content_type: "Embed"
  embed_code: |
    <div class="calendly-inline-widget"
      data-url="https://calendly.com/yourname/30min"
      style="min-width:320px;height:630px;">
    </div>
```

#### Example 4: Video Tab

```yaml
Tab Configuration:
  type: "Videos (Youtube Links)"
  title: "Demo"
  description: "Product walkthrough video"
  content_type: "Embed"
  embed_url: "https://www.youtube.com/embed/YOUR_VIDEO_ID"
```

### Adding Multiple Tabs

**Add Tab Button:**

After configuring your first tab, click **[+ Add Tab]** at the bottom to add more:

```
Workflow:
1. Click [+ Add Tab]
2. Select tab type from dropdown
3. Configure tab settings
4. Click [+ Add Tab] again for next tab
5. Repeat until all tabs are configured
```

**Tab Order:**

Drag tabs to reorder them:

```
Before:                After Reordering:
┌────────────┐        ┌────────────┐
│ ⋮⋮ Welcome │        │ ⋮⋮ Welcome │
│ ⋮⋮ Buy Now │  →     │ ⋮⋮ Chat    │
│ ⋮⋮ Chat    │        │ ⋮⋮ Buy Now │
│ ⋮⋮ Calendar│        │ ⋮⋮ Calendar│
└────────────┘        └────────────┘
```

!!! tip "Tab Organization"
    Place most important tabs first (left in horizontal, top in vertical). Users often click the first 2-3 tabs most.

### Preview Mode

**Preview Options:**

```
┌──────────────────────────────────────┐
│  [Mobile] [Desktop] [Maximize]       │
├──────────────────────────────────────┤
│                                      │
│     Live Preview of IQ Bot           │
│     with configured tabs             │
│                                      │
└──────────────────────────────────────┘
```

**Preview Modes:**
- **Mobile** - Phone view (320-480px)
- **Desktop** - Full desktop view
- **Maximize** - Full screen preview

Test your IQ Bot in different views before going live!

---

## Step 4: Review and Test

### Test Your Configuration

Before activating, verify:

- ✅ All required fields completed
- ✅ AI Bot selected
- ✅ At least 2-3 tabs configured
- ✅ All URLs are valid and working
- ✅ Embed codes display correctly
- ✅ Tab order is logical
- ✅ Button text is clear and actionable
- ✅ Preview looks good on mobile and desktop

### Test Each Tab

**Testing Checklist:**

```
Tab Testing:
├─ Welcome Tab
│  └─ Content displays correctly
├─ Chat Tab
│  ├─ AI Bot loads
│  ├─ Can send test messages
│  └─ Responses are accurate
├─ Calendar Tab
│  ├─ Calendar widget loads
│  └─ Can select time slots
├─ Video Tab
│  ├─ Video plays
│  └─ Controls work
├─ Buy Now Tab
│  ├─ Links open correctly
│  └─ Buttons are clickable
└─ Custom Tabs
   └─ Forms and content function properly
```

### Common Issues

**Issue: "At least one valid link URL is required"**
```
Solution:
1. Ensure URL starts with https://
2. Check for typos in URL
3. Remove any extra spaces
4. Verify URL is accessible
```

**Issue: "Button text is required"**
```
Solution:
1. Fill in button text for each link
2. Ensure text is not empty
3. Check all buttons have text
```

**Issue: Embed not displaying**
```
Solution:
1. Check if site allows embedding
2. Try Link instead of Embed
3. Verify iframe code is complete
4. Test embed URL in browser first
```

---

## Step 5: Activate and Share

### Save Your IQ Bot

After configuring all settings and tabs:

```
[Save] or [Save & Activate]
```

**Save Options:**
- **Save** - Saves as Inactive (for testing)
- **Save & Activate** - Saves and makes live immediately

!!! tip "Save as Inactive First"
    Save as Inactive, test the URL, then activate once everything works perfectly.

### Access Your IQ Bot

Once saved, your IQ Bot is assigned a URL:

```
┌─────────────────────────────────────────┐
│  Your IQ Bot is Ready!                  │
├─────────────────────────────────────────┤
│                                         │
│  URL: https://test.iquivity.net/iqbot/ │
│       adbot1                            │
│                                         │
│  QR Code:                               │
│  ┌─────────┐                           │
│  │ ▄▄▄▄▄▄▄ │                           │
│  │ █     █ │                           │
│  │ █ ███ █ │                           │
│  │ █ ███ █ │                           │
│  │ █     █ │                           │
│  │ ▀▀▀▀▀▀▀ │                           │
│  └─────────┘                           │
│                                         │
│  [Download QR Code]                     │
│  [Copy URL]                             │
│  [Share]                                │
│                                         │
└─────────────────────────────────────────┘
```

### Activate Your IQ Bot

**From Dashboard:**

```
IQ Bots Dashboard
  → Inactive IQBots
    → [Your Bot] → ⋮ Menu
      → Activate
```

**Action Menu (⋮):**
```
├── Edit        - Modify settings
├── Analytics   - View metrics
├── Share       - Get URL/QR code
├── Activate    - Make live ✓
└── Delete      - Remove bot
```

**Activation Confirmation:**

```
┌────────────────────────────────────┐
│  Activate IQ Bot?                  │
├────────────────────────────────────┤
│                                    │
│  Your IQ Bot will become publicly  │
│  accessible via its URL.           │
│                                    │
│  URL: test.iquivity.net/iqbot/     │
│       adbot1                       │
│                                    │
│  [Cancel]  [Activate]              │
│                                    │
└────────────────────────────────────┘
```

Once activated:
- IQ Bot moves to "Active IQBots" section
- URL becomes publicly accessible
- QR code can be downloaded and shared
- Analytics start tracking visitors

### Share Your IQ Bot

**Sharing Options:**

**1. Direct URL:**
```
https://test.iquivity.net/iqbot/adbot1
```

**Share in:**
- Email campaigns
- Social media posts
- Website links
- Email signatures
- Text messages
- Slack/Teams messages

**2. QR Code:**

Download the QR code and use on:
- Business cards
- Flyers and brochures
- Posters and signage
- Product packaging
- Event materials
- Print advertising
- In-store displays
- Presentation slides

**3. Share Button:**

Use the built-in share function to:
- Copy URL to clipboard
- Generate social media posts
- Create email templates
- Download QR code
- Get embed code (if available)

---

## Managing Your IQ Bot

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
│  [Empty state]                                 │
│                                                │
│  Inactive IQBots (2)                           │
│  [Search Inactive IQ bots]                     │
│  ┌──────────────┐  ┌──────────────┐           │
│  │ Adbot1       │  │ Trading Bot  │           │
│  │ Created 107  │  │ Created 107  │           │
│  │ days ago     │  │ days ago  ⋮ │           │
│  │              │  │              │           │
│  │ URL + QR     │  │ URL + QR     │           │
│  │ [Download]   │  │ [Download]   │           │
│  └──────────────┘  └──────────────┘           │
│                                                │
│  Deleted IQBots (0)                            │
│  [Empty state]                                 │
│                                                │
└────────────────────────────────────────────────┘
```

### Bot Actions

**Available Actions (⋮ Menu):**

```
Bot Actions:
├── Edit
│   └─ Modify General settings, tabs
├── Analytics
│   └─ View detailed usage metrics
├── Share
│   └─ Access URL and QR code
├── Activate / Deactivate
│   └─ Toggle bot status
└── Delete
    └─ Move to deleted (30-day recovery)
```

#### Edit

**Modify Bot Settings:**

```
Edit Menu → Opens configuration pages:
├─ General Settings
│  ├─ Change name (if not yet used)
│  ├─ Update description
│  ├─ Switch AI Bot
│  ├─ Change tab orientation
│  └─ Update logo
└─ Tabs
   ├─ Add new tabs
   ├─ Edit existing tabs
   ├─ Reorder tabs
   └─ Delete tabs
```

!!! warning "Changes to Active Bots"
    Changes to active IQ Bots take effect immediately. Preview before saving.

#### Analytics

**View Performance Metrics:**

```
Analytics Dashboard:
├─ Daily / Weekly / Monthly / Custom views
├─ Total Tab Views
├─ Average Time Spent on Tab
├─ Daily Tab Clicks
├─ IQ Bot Interactions (chart)
├─ Popular Tabs (ranking)
├─ Geographic Analytics
└─ Platform Breakdown
```

See [Analytics Guide](../ai-bot/analytics.md) for detailed information.

#### Share

**Access Sharing Options:**

```
Share Panel:
├─ Copy URL to clipboard
├─ Download QR Code (PNG)
├─ Email sharing template
├─ Social media posts
└─ Embed code (if available)
```

#### Activate / Deactivate

**Toggle Bot Status:**

```
Status Toggle:
Active → [Deactivate] → Inactive
Inactive → [Activate] → Active
```

**When Inactive:**
- URL returns "inactive" message
- Not accessible to public
- Can still be edited and tested
- Analytics not tracking

**When Active:**
- URL is publicly accessible
- QR code works
- Analytics tracking enabled
- All features live

#### Delete

**Remove IQ Bot:**

```
Delete Process:
1. Click Delete
2. Confirm deletion
3. Bot moves to "Deleted IQBots"
4. 30-day recovery period
5. Permanent deletion after 30 days
```

**Deleted Bot Actions:**
```
Deleted IQBots:
├── Restore
│   └─ Moves back to Inactive
└── Delete Permanently
    └─ Immediate permanent deletion
```

!!! danger "Permanent Deletion"
    After 30 days or manual permanent deletion, IQ Bots cannot be recovered. All tabs and settings are lost.

---

## Best Practices

### Tab Strategy

**Recommended Tab Combinations:**

**Basic (3-4 tabs):**
```
┌─────────┬──────┬──────────┬─────────┐
│ Welcome │ Chat │ Calendar │ Buy Now │
└─────────┴──────┴──────────┴─────────┘
```

**Standard (5-6 tabs):**
```
┌─────────┬──────┬──────────┬───────┬──────┬──────┐
│ Welcome │ Chat │ Calendar │ Video │ Docs │ Buy  │
└─────────┴──────┴──────────┴───────┴──────┴──────┘
```

**Comprehensive (7+ tabs):**
```
┌─────────┬──────┬──────────┬───────┬──────┬──────┬─────────┬────────┐
│ Welcome │ Chat │ Calendar │ Video │ Docs │ Buy  │ Reviews │ Custom │
└─────────┴──────┴──────────┴───────┴──────┴──────┴─────────┴────────┘
```

### Content Guidelines

**Welcome Tab:**
- Brief introduction (2-3 sentences)
- Clear value proposition
- Visual elements (logo, images)
- Call-to-action

**Chat Tab:**
- Pre-configure AI Bot thoroughly
- Test common questions
- Set up human handoff
- Add office hours message

**Calendar Tab:**
- Use reputable scheduling tools
- Show availability clearly
- Include time zone
- Add confirmation messages

**Buy Now Tab:**
- Clear product information
- Multiple payment options
- Secure checkout process
- Mobile-optimized

### URL and QR Code Usage

**URL Best Practices:**
- Use short, memorable bot names
- Include in email signatures
- Add to social media bios
- Link from website footer
- Include in marketing materials

**QR Code Best Practices:**
- Download high-resolution version
- Test before printing
- Place at eye level
- Include short text instructions
- Use contrasting background
- Ensure adequate size (minimum 2cm x 2cm)

### Testing Checklist

Before activating:

- [ ] AI Bot responds correctly
- [ ] All tabs load properly
- [ ] Links open in correct mode (new tab/embed)
- [ ] Embed codes display correctly
- [ ] Button text is clear
- [ ] Mobile view works well
- [ ] Desktop view is optimized
- [ ] Tab order makes sense
- [ ] Logo displays properly
- [ ] QR code scans correctly
- [ ] URL is accessible
- [ ] All forms submit successfully

---

## Troubleshooting

### Common Issues and Solutions

**Issue: "No AI Bot available in dropdown"**
```
Cause: No AI Bot created yet
Solution:
1. Navigate to AI Bot section
2. Create new AI Bot
3. Train it on your data
4. Return to IQ Bot creation
5. Select your AI Bot from dropdown
```

**Issue: Tab not displaying content**
```
Cause: Incorrect embed code or URL
Solution:
1. Verify URL is accessible
2. Check for typos
3. Try "Link" instead of "Embed"
4. Test URL in browser first
5. Check X-Frame-Options on external site
```

**Issue: QR code not generating**
```
Cause: Bot not saved yet
Solution:
1. Save IQ Bot first
2. QR code generates automatically
3. Access from Share menu
4. Download from Inactive/Active bot card
```

**Issue: Can't reorder tabs**
```
Cause: Not using drag handle
Solution:
1. Click ⋮⋮ drag handle on left of tab
2. Drag up or down
3. Release when in desired position
4. Save changes
```

**Issue: Changes not reflecting**
```
Cause: Cache or not saved
Solution:
1. Ensure you clicked Save
2. Hard refresh browser (Ctrl+Shift+R)
3. Clear browser cache
4. Try incognito/private mode
5. Check if bot is Active
```

**Issue: Analytics showing zero**
```
Cause: Bot is inactive or no visits yet
Solution:
1. Activate bot
2. Visit URL to test
3. Wait 1-2 hours for data processing
4. Check if tracking is enabled
5. Verify bot is publicly accessible
```

---

## Next Steps

Congratulations! Your IQ Bot is now live. Here's what to do next:

### Monitor Performance

**Track Key Metrics:**
```
Week 1:
├─ Monitor which tabs get most clicks
├─ Check average time on each tab
├─ Review chat interactions
└─ Identify any issues

Week 2-4:
├─ Analyze popular tabs
├─ Optimize underperforming tabs
├─ A/B test different content
└─ Add new tabs based on data
```

### Optimize Content

**Continuous Improvement:**
- Review analytics weekly
- Update content based on feedback
- Add new tabs for emerging needs
- Remove low-performing tabs
- Test different tab orders
- Improve AI Bot responses

### Scale Your Usage

**Expand Your IQ Bot Strategy:**
- Create multiple IQ Bots for different campaigns
- Use for events, products, services
- Integrate with marketing automation
- Track ROI and conversions
- Share best practices with team

---

!!! success "You're All Set!"
    Your IQ Bot is now live and ready to engage users. Monitor analytics, gather feedback, and continuously improve your mini-site.

**Need Help?** Contact support at support@iquivity.ai

**Last Updated:** December 6, 2025 | **Version:** 2.0
