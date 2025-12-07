# Marketing Bot - Campaigns

Create, manage, and track broadcast message campaigns across WhatsApp and Telegram platforms.

---

## Overview

Campaigns allow you to broadcast messages to multiple contacts simultaneously on WhatsApp and Telegram. Schedule promotional messages, announcements, and engagement campaigns to reach your entire audience instantly.

!!! info "Platform-Specific Campaigns"
    Campaigns are organized by platform. Create separate campaigns for WhatsApp and Telegram to leverage platform-specific features.

---

## Campaign Types

### WhatsApp Campaigns

Broadcast messages to WhatsApp contacts with rich media support, delivery tracking, and engagement analytics.

**WhatsApp Campaign Features:**
- Text and media messages
- Broadcast lists
- Delivery receipts
- Read status tracking
- Training status monitoring
- Schedule at specific times

### Telegram Campaigns

Send messages to Telegram groups, channels, and individual subscribers with bot automation and interactive elements.

**Telegram Campaign Features:**
- Group broadcasting
- Channel posts
- Direct messages
- Bot commands
- Inline buttons
- Schedule future sends

---

## WhatsApp Campaigns

### Campaign List View

**Display Columns:**

| ID | Name | Status | Training | Schedule At | Action |
|----|------|--------|----------|-------------|--------|
| 1 | Summer Super Sale | ✅ Published | Not Trained | 2029-06-13 11:24 | ⚡ ✏️ ✕ |
| 2 | VIP Member Free Trial Week | ✅ Published | Not Trained | 2025-06-03 11:57 | ⚡ ✏️ ✕ |
| 3 | Flash Offer – 50% Off Today | ✅ Published | Not Trained | 2025-06-05 17:57 | ⚡ ✏️ ✕ |
| 4 | New Product Launch – Special Invite | ✅ Published | Not Trained | 2027-06-05 17:57 | ⚡ ✏️ ✕ |
| 5 | Webinar Registration Now Open | ✅ Published | Not Trained | 2027-06-05 17:57 | ⚡ ✏️ ✕ |

**Example Campaigns:**
```
WhatsApp Campaigns (5 total)

1. Summer Super Sale
   Status: Published
   Training: Not Trained
   Scheduled: 2029-06-13 11:24

2. VIP Member Free Trial Week
   Status: Published
   Training: Not Trained
   Scheduled: 2025-06-03 11:57

3. Flash Offer – 50% Off Today
   Status: Published
   Training: Not Trained
   Scheduled: 2025-06-05 17:57
```

---

## Telegram Campaigns

### Campaign List View

**Display Columns:**

| ID | Name | Status | Schedule At | Action |
|----|------|--------|-------------|--------|
| 6 | Exclusive Telegram Deal | 🕐 Scheduled | 2029-06-13 11:24 | ✏️ ✕ |
| 7 | Weekend Special Offer | ✅ Published | 2025-06-03 11:57 | ✏️ ✕ |
| 8 | Join Our Premium Membership | ✅ Published | 2025-06-05 17:57 | ✏️ ✕ |
| 9 | Holiday Season Price Drop | 🕐 Scheduled | 2027-06-05 17:57 | ✏️ ✕ |
| 10 | Early Bird Special Discount | 🕐 Scheduled | 2027-06-05 17:57 | ✏️ ✕ |

**Example Campaigns:**
```
Telegram Campaigns (5 total)

6. Exclusive Telegram Deal
   Status: Scheduled
   Scheduled: 2029-06-13 11:24

7. Weekend Special Offer
   Status: Published
   Scheduled: 2025-06-03 11:57

8. Join Our Premium Membership
   Status: Published
   Scheduled: 2025-06-05 17:57
```

---

## Campaign Status Types

### Status Indicators

**Published (✅):**
- Campaign has been sent
- Messages delivered to contacts
- Analytics available
- Cannot be edited (can duplicate)
- Delivery tracking active

**Scheduled (🕐):**
- Campaign queued for future send
- Awaiting scheduled time
- Can be edited before send
- Can be rescheduled
- Can be canceled

**Draft:**
- Campaign being created
- Not yet scheduled
- Can be fully edited
- Not visible to contacts
- Awaiting completion

**Failed (❌):**
- Campaign send failed
- Error occurred during delivery
- Requires attention
- Can be retried
- Check logs for details

---

## Creating New Campaign

### Campaign Creation Button

**Add Campaign Button:** **"+ Add campaign"**

Located in top-right corner for easy access.

---

### Campaign Setup Form

#### Step 1: Campaign Details

**Basic Information:**

```
Campaign Name: [Enter campaign name]
  Example: "Flash Sale Weekend Offer"

Platform: [Select ▼]
  ○ WhatsApp
  ○ Telegram

Campaign Type: [Select ▼]
  - Promotional
  - Informational
  - Event Announcement
  - Follow-up
  - Engagement
```

---

#### Step 2: Target Audience

**Audience Selection:**

```
Select Recipients:
☑ All Contacts
☐ Specific Segments
☐ Custom List
☐ Import from File

Segments (if applicable):
☐ VIP Customers
☐ New Leads
☐ Repeat Buyers
☐ Inactive Customers
☐ Webinar Participants

Estimated Reach: 156 contacts
```

**For Telegram:**
```
Broadcast To:
☐ All Subscribers
☐ Specific Groups
☐ Channel Members
☐ Direct Messages

Select Groups:
☐ Tech Lovers
☐ Marketing Gurus
☐ Startup Founders
☐ Fitness Enthusiasts
☐ Book Club
☐ Crypto Traders
```

---

#### Step 3: Message Content

**Message Composition:**

**Text Content:**
```
┌────────────────────────────────────┐
│ Message Text                       │
│                                    │
│ [Compose your message here]       │
│                                    │
│ Maximum 4,096 characters          │
│ Supports emojis and formatting    │
│                                    │
└────────────────────────────────────┘

Character Count: 0 / 4,096
```

**Message Example:**
```
Flash Sale! 🔥

Get up to 50% off on all items. Hurry, limited time offer!
Shop now and save big.

Use code: FLASH50
Valid until: [Date]

Shop now: [Link]

#FlashSale #LimitedTimeOffer
```

**Media Attachments:**
```
Add Media:
├── Image (JPG, PNG, GIF)
├── Video (MP4, up to 16MB)
├── Document (PDF, DOC)
└── Link Preview

[+ Upload Media]

Current Attachments:
└── flash-sale-banner.jpg (1.2 MB)
```

**Formatting Options:**
- **Bold text**: `*text*`
- _Italic text_: `_text_`
- `Monospace`: `` `text` ``
- ~~Strikethrough~~: `~text~`
- Links: `[Link Text](URL)`

---

#### Step 4: Schedule Campaign

**Scheduling Options:**

**Send Immediately:**
```
○ Send Now
  Campaign will be broadcast immediately after creation
```

**Schedule for Later:**
```
☑ Schedule Send

Date: [Date Picker]
  Example: 2025-06-05

Time: [Time Picker]
  Example: 17:57

Time Zone: [Select ▼]
  - UTC
  - America/New_York
  - Europe/London
  - Asia/Tokyo
  - etc.
```

**Repeat Options:**
```
Recurring Campaign:
☐ Enable Recurring

Frequency:
  - Daily
  - Weekly
  - Monthly
  - Custom

End Date: [Date Picker]
```

---

#### Step 5: Advanced Settings

**Delivery Options:**

**WhatsApp Settings:**
```
Broadcast Settings:
☑ Split into broadcast lists (max 256 per list)
☑ Track delivery status
☑ Track read receipts
☐ Send test message first

Throttling:
Max messages per minute: [50]
Delay between batches: [2 seconds]
```

**Telegram Settings:**
```
Message Options:
☑ Disable link preview
☐ Disable notifications
☐ Pin message
☑ Add inline keyboard

Bot Commands:
☐ Enable bot interactions
Reply Markup: [None ▼]
```

**Training Status:**
```
AI Training:
○ Not Trained (default)
○ Train for responses
○ Use trained model

Training Note: WhatsApp campaigns show "Not Trained"
status by default. Enable training for automated responses.
```

---

#### Step 6: Review and Confirm

**Campaign Summary:**

```
┌─────────────────────────────────────┐
│ Campaign Review                     │
├─────────────────────────────────────┤
│ Name: Flash Offer – 50% Off Today  │
│ Platform: WhatsApp                  │
│ Status: Scheduled                   │
│ Recipients: 156 contacts            │
│ Schedule: 2025-06-05 17:57         │
│ Training: Not Trained               │
│                                     │
│ Message Preview:                    │
│ Flash Sale! 🔥                     │
│ Get up to 50% off...               │
│                                     │
│ [Media: flash-sale-banner.jpg]     │
│                                     │
│ [Edit] [Send Test] [Schedule]      │
└─────────────────────────────────────┘
```

**Action Buttons:**
- **Edit**: Modify campaign details
- **Send Test**: Send to test numbers
- **Schedule**: Confirm and schedule
- **Save Draft**: Save for later

---

## Campaign Actions

### Managing Campaigns

**Available Actions:**

**Star/Feature (⚡):**
- Mark campaign as featured
- Priority in list
- Quick access
- Available only for WhatsApp campaigns

**Edit (✏️):**
- Modify campaign details
- Only for scheduled campaigns
- Cannot edit published campaigns
- Update message content
- Change schedule time

**Delete (✕):**
- Remove campaign permanently
- Confirm before deletion
- Cannot be undone
- Scheduled campaigns can be deleted
- Published campaigns archived

**Duplicate:**
- Create copy of campaign
- Reuse successful campaigns
- Modify and resend
- Save time on creation
- Available from menu

---

## Campaign Management

### Campaign List Features

**Search Campaigns:**
```
🔍 Search by:
├── Campaign name
├── Status
├── Date range
├── Platform
└── Training status
```

**Filter Options:**
```
Filter By:
├── Status (All, Published, Scheduled, Draft, Failed)
├── Platform (All, WhatsApp, Telegram)
├── Training (All, Trained, Not Trained)
└── Date Range (Today, This Week, This Month, Custom)
```

**Sort Options:**
```
Sort By:
├── Most Recent
├── Oldest First
├── Name (A-Z)
├── Name (Z-A)
├── Schedule Date
└── Status
```

**Bulk Actions:**
```
☑ Select Multiple Campaigns

Bulk Actions:
├── Delete Selected
├── Change Status
├── Export List
├── Duplicate Selected
└── Update Training Status
```

---

## WhatsApp-Specific Features

### Broadcast Lists

**WhatsApp Limitations:**
- Maximum 256 contacts per broadcast
- Auto-split for larger audiences
- Individual delivery per contact
- Recipients don't see other contacts

**Broadcast Management:**
```
Broadcast Settings:
Total Contacts: 512
Broadcast Lists: 2 (256 each)

List 1: Contacts 1-256
List 2: Contacts 257-512
```

### Training Status

**Training Options:**

**Not Trained (Default):**
- Standard broadcast only
- One-way communication
- No automated responses
- Manual reply handling

**Trained:**
- AI-powered responses
- Auto-reply to common questions
- Smart routing
- Enhanced engagement

**Training Setup:**
```
1. Enable training in campaign settings
2. Define response triggers
3. Set up response templates
4. Test AI responses
5. Monitor and improve
```

---

## Telegram-Specific Features

### Group Broadcasting

**Telegram Groups:**

Manage broadcasting to multiple groups:

**Available Groups:**
```
ID | Group Name | Members
---|------------|--------
1  | Tech Lovers | 2,450
2  | Marketing Gurus | 1,823
3  | Startup Founders | 945
4  | Fitness Enthusiasts | 3,102
5  | Book Club | 567
6  | Crypto Traders | 4,891
```

**Group Selection:**
```
☑ Select All Groups
☐ Tech Lovers (2,450 members)
☑ Marketing Gurus (1,823 members)
☐ Startup Founders (945 members)
☑ Fitness Enthusiasts (3,102 members)
☐ Book Club (567 members)
☐ Crypto Traders (4,891 members)

Total Reach: 6,748 members
```

### Subscribers Management

**View Group Subscribers:**

**Subscriber List:**
```
ID | Name | Username | Action
---|------|----------|-------
1  | John Doe | @john_doe | ✕
2  | Jane Smith | @jane_smith | ✕
3  | Mike Johnson | @mike_johnson | ✕
4  | Emily Davis | @emily_davis | ✕
5  | Robert Wilson | @robert_wilson | ✕
6  | Laura Brown | @laura_brown | ✕
7  | Daniel Miller | @daniel_miller | ✕
```

**Subscriber Actions:**
- View subscriber details
- Remove from group
- Block user
- Export list
- Send direct message
- Add to segment

---

## Campaign Analytics

### Performance Metrics

**WhatsApp Campaign Stats:**
```
Campaign: Flash Offer – 50% Off Today
─────────────────────────────────────
Sent:        156 messages
Delivered:   154 (98.7%)
Failed:      2 (1.3%)
Read:        128 (82.1%)
Clicked:     45 (28.8%)
Responses:   23 (14.7%)
```

**Telegram Campaign Stats:**
```
Campaign: Weekend Special Offer
─────────────────────────────────────
Sent:        6,748 messages
Delivered:   6,742 (99.9%)
Failed:      6 (0.1%)
Views:       5,234 (77.6%)
Clicks:      892 (13.2%)
Shares:      156 (2.3%)
```

### Delivery Reports

**Detailed Analytics:**

**Delivery Status:**
| Status | Count | Percentage |
|--------|-------|------------|
| Delivered | 154 | 98.7% |
| Read | 128 | 82.1% |
| Failed | 2 | 1.3% |
| Pending | 0 | 0% |

**Failure Reasons:**
- Invalid number: 1
- Blocked contact: 0
- Network error: 1
- Platform restriction: 0

**Engagement Metrics:**
- Click-through rate: 28.8%
- Response rate: 14.7%
- Conversion rate: 5.1%
- Average response time: 15 minutes

---

## Best Practices

### Campaign Strategy

**Content Guidelines:**
- ✅ Keep messages concise and clear
- ✅ Include strong call-to-action
- ✅ Use engaging visuals
- ✅ Personalize when possible
- ✅ Test before broadcasting

**Timing Recommendations:**
- 📅 Schedule during business hours (9 AM - 7 PM)
- ⏰ Avoid early morning (before 8 AM)
- 🌙 Avoid late night (after 9 PM)
- 📊 Test different times to find optimal
- 🔄 Review analytics to optimize

**Compliance:**
- ⚖️ Follow platform policies
- 📜 Obtain user consent
- 🚫 Provide opt-out option
- 🔒 Protect user privacy
- ✅ Honor unsubscribe requests

**Engagement Tips:**
- 💬 Encourage replies
- 🎁 Offer exclusive deals
- 🎯 Target relevant segments
- 📸 Use high-quality images
- 🔗 Include trackable links

---

## Campaign Templates

### Pre-built Campaign Types

**Promotional Campaigns:**
```
Template: Flash Sale
Message: "Flash Sale! 🔥 Get up to [X]% off on [products].
Limited time offer! Use code: [CODE]"

Template: New Product Launch
Message: "Introducing [Product Name]! Be among the first
to try it. Exclusive launch offer: [Discount]"
```

**Engagement Campaigns:**
```
Template: Survey Request
Message: "We value your feedback! Help us improve by
taking our 2-minute survey: [Link]"

Template: Event Invitation
Message: "You're invited! Join us for [Event Name] on
[Date]. Register now: [Link]"
```

**Transactional Campaigns:**
```
Template: Order Confirmation
Message: "Order confirmed! Your order #[ID] will be
delivered on [Date]. Track: [Link]"

Template: Appointment Reminder
Message: "Reminder: You have an appointment on [Date]
at [Time]. Location: [Address]"
```

---

## Troubleshooting

### Common Issues

**Campaign Not Sending:**
- **Cause:** Invalid API credentials, platform restrictions, no recipients selected
- **Solution:** Check settings, verify tokens, ensure contacts selected

**Low Delivery Rate:**
- **Cause:** Invalid numbers, blocked contacts, network issues
- **Solution:** Clean contact list, verify numbers, check connectivity

**Messages Failing:**
- **Cause:** Platform limits exceeded, content violations, technical errors
- **Solution:** Review platform policies, reduce send rate, check error logs

**Schedule Not Working:**
- **Cause:** Incorrect time zone, past date selected, system time mismatch
- **Solution:** Verify time zone, use date picker, check system clock

**Training Status Not Updating:**
- **Cause:** Training not enabled, insufficient data, processing delay
- **Solution:** Enable training in settings, provide training data, wait for processing

---

## Next Steps

<div class="grid cards" markdown>

-   :fontawesome-brands-telegram:{ .lg .middle } __Telegram Setup__

    ---

    Configure Telegram groups and subscribers

    [:octicons-arrow-right-24: Telegram](telegram.md)

-   :fontawesome-brands-whatsapp:{ .lg .middle } __WhatsApp Setup__

    ---

    Manage WhatsApp contacts and lists

    [:octicons-arrow-right-24: WhatsApp](whatsapp.md)

-   :material-cog:{ .lg .middle } __Bot Settings__

    ---

    Configure API tokens and webhooks

    [:octicons-arrow-right-24: Settings](settings.md)

</div>

---

**Previous:** [← Inbox](inbox.md) | **Next:** [Telegram →](telegram.md)

---

**Last Updated:** December 2025
