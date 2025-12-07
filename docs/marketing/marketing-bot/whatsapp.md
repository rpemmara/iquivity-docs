# Marketing Bot - WhatsApp

Manage WhatsApp contacts, contact lists, segments, and broadcast campaigns for automated messaging.

---

## Overview

The WhatsApp integration enables you to manage contacts, organize them into lists and segments, and broadcast messages to your WhatsApp audience. Leverage WhatsApp's business features for customer engagement and marketing automation.

!!! info "WhatsApp Business API"
    Connect via WhatsApp Business API to unlock advanced features like automated messages, broadcast lists, and rich media support.

---

## Contact Lists

### Manage Contact Lists

**Contact Lists View:**

| ID | Name | Action |
|----|------|--------|
| 1 | John Doe | ✕ |
| 2 | Jane Smith | ✕ |
| 3 | Mike Johnson | ✕ |
| 4 | Emily Davis | ✕ |
| 5 | Robert Wilson | ✕ |
| 6 | Laura Brown | ✕ |

**List Information:**
- List ID and name
- Number of contacts
- Creation date
- Last updated
- Status (active/inactive)

**List Actions:**
- **Remove (✕)**: Delete contact list
- **Edit**: Update list details
- **Export**: Download contact data
- **Duplicate**: Create copy of list
- **Merge**: Combine with another list

---

## Adding Contacts

### Add New Contact

**Manual Entry:**
```
1. Click "+ Add Contact" button
2. Enter contact details:
   - Name: [Contact Name]
   - Phone: [+Country Code + Number]
   - Email: [optional]
   - Tags: [optional]
3. Assign to list or segment
4. Save contact
```

**Bulk Import:**
```
1. Prepare CSV file with columns:
   - Name, Phone, Email, Tags
2. Click "Import Contacts"
3. Select CSV file
4. Map columns
5. Review and import
6. Verify imported contacts
```

**CSV Format Example:**
```
Name,Phone,Email,Tags
John Doe,+12035550101,john@example.com,VIP
Jane Smith,+442083661234,jane@example.com,Lead
Mike Johnson,+493012345678,mike@example.com,Customer
```

---

## Contacts Management

### View All Contacts

**Contacts List View:**

| ID | Name | Phone | Action |
|----|------|-------|--------|
| 1 | John Doe | +12035550101 | ✕ |
| 2 | Jane Smith | +442083661234 | ✕ |
| 3 | Mike Johnson | +493012345678 | ✕ |
| 4 | Emily Davis | +12035550123 | ✕ |
| 5 | Robert Wilson | +442071838750 | ✕ |

**Contact Details:**
- Contact ID
- Full name
- Phone number (with country code)
- Email address
- Tags/segments
- Join date
- Last interaction
- Message count

**Contact Actions:**
- **Remove (✕)**: Delete contact
- **Edit**: Update contact information
- **Message**: Send direct message
- **View History**: See conversation history
- **Add to Segment**: Organize contact
- **Block**: Prevent messaging

---

## Contact Segments

### Organize Contacts into Segments

**Segments List View:**

| ID | Name | Action |
|----|------|--------|
| 1 | VIP Customers | ✕ |
| 2 | New Leads | ✕ |
| 3 | Repeat Buyers | ✕ |
| 4 | Inactive Customers | ✕ |
| 5 | Webinar Participants | ✕ |

**Segment Information:**
- Segment name
- Number of contacts
- Segment criteria
- Creation date
- Last updated

**Segment Actions:**
- **Remove (✕)**: Delete segment
- **Edit**: Modify segment criteria
- **View Contacts**: See segment members
- **Broadcast**: Send campaign to segment
- **Export**: Download segment data

---

## Creating Segments

### Build Custom Segments

**Segment Criteria:**

**By Behavior:**
```
Create segment based on:
├── Purchase history
├── Message engagement
├── Website visits
├── Cart abandonment
└── Email opens/clicks
```

**By Demographics:**
```
Filter by:
├── Location/Country
├── Age range
├── Gender
├── Language
└── Time zone
```

**By Tags:**
```
Include contacts with tags:
☐ VIP
☐ Lead
☐ Customer
☐ Prospect
☐ Partner
```

**Dynamic Segments:**
```
Auto-update based on:
├── Recent purchase (last 30 days)
├── Active users (messaged in last 7 days)
├── High spenders (>$500 total)
├── Inactive (no message in 90 days)
└── Birthday this month
```

---

## Broadcasting to Contacts

### Send Messages to WhatsApp Contacts

**Broadcast Options:**

**Select Recipients:**
```
Target Audience:
☐ All Contacts
☐ Specific List
☐ Segment
☐ Custom Selection

Selected Contacts: 156
Estimated Reach: 154 (98.7%)
```

**Message Composition:**
```
┌────────────────────────────────────┐
│ Message Text                       │
│                                    │
│ Flash Sale! 🔥                    │
│ Get up to 50% off on all items.   │
│ Limited time offer!                │
│                                    │
│ Use code: FLASH50                  │
│ Shop now: [Link]                   │
│                                    │
└────────────────────────────────────┘

[+ Add Media] [+ Add Template] [Send]
```

**Media Types:**
- Images (JPG, PNG)
- Videos (MP4, max 16MB)
- Documents (PDF, DOC)
- Audio files
- Location
- Contact cards

---

## WhatsApp Templates

### Message Templates

**Pre-approved Templates:**

WhatsApp requires pre-approved templates for business messages:

**Template Categories:**
- Promotional offers
- Order notifications
- Appointment reminders
- Shipping updates
- Payment confirmations
- Customer support

**Creating Templates:**
```
1. Navigate to Settings > Templates
2. Click "+ New Template"
3. Define template structure:
   - Name: flash_sale_offer
   - Category: Promotional
   - Language: English
   - Body: Your message text with {{variables}}
4. Submit for approval
5. Wait for WhatsApp approval (24-48 hours)
6. Use approved template in campaigns
```

**Template Example:**
```
Template Name: flash_sale_offer
Category: Promotional

Body:
Hello {{1}},

Flash Sale Alert! 🔥
Get {{2}}% off on all items.
Use code: {{3}}

Valid until: {{4}}
Shop now: {{5}}

Reply STOP to unsubscribe.
```

---

## WhatsApp Business Features

### Business Profile

**Profile Settings:**
```
Business Name: [Your Business]
Category: [Select Industry]
Description: [Business Description]
Address: [Business Address]
Website: [URL]
Email: [Contact Email]
Hours: [Business Hours]
```

**Profile Photo:**
- Upload logo (640x640px recommended)
- Displays in chats
- Builds brand recognition

**Catalog Integration:**
- Link product catalog
- Share products in chat
- Enable shopping features

---

## Broadcast Lists

### WhatsApp Broadcast Lists

**List Limitations:**
- Maximum 256 contacts per list
- Recipients must have your number saved
- Messages appear as individual chats
- Recipients don't see other members

**Creating Broadcast List:**
```
1. Select up to 256 contacts
2. Click "Create Broadcast List"
3. Name the list
4. Send message to list
5. Track delivery status
```

**Auto-Split for Large Audiences:**
```
Total Contacts: 512
Auto-creates:
├── Broadcast List 1: 256 contacts
└── Broadcast List 2: 256 contacts

Messages sent sequentially to both lists
```

---

## WhatsApp Analytics

### Performance Tracking

**Message Metrics:**
```
Campaign: Flash Offer - 50% Off Today
─────────────────────────────────────
Sent:        156 messages
Delivered:   154 (98.7%)
Read:        128 (82.1%)
Failed:      2 (1.3%)
Replied:     23 (14.7%)
```

**Delivery Status:**
| Status | Count | Percentage |
|--------|-------|------------|
| Delivered | 154 | 98.7% |
| Read | 128 | 82.1% |
| Pending | 0 | 0% |
| Failed | 2 | 1.3% |

**Engagement Metrics:**
- Open rate: 82.1%
- Reply rate: 14.7%
- Click-through rate: 28.8%
- Conversion rate: 5.1%
- Average response time: 15 min

---

## WhatsApp Automation

### Automated Workflows

**Auto-Responses:**
```
Trigger: Customer message received
Response: Welcome message
Delay: Immediate

Trigger: Keyword "price"
Response: Send pricing information
Delay: 2 seconds

Trigger: Business hours end
Response: "We're offline, will reply tomorrow"
Delay: Immediate
```

**Follow-up Sequences:**
```
Day 1: Welcome message
Day 3: Product information
Day 7: Special offer
Day 14: Feedback request
Day 30: Re-engagement message
```

**Event-Based Triggers:**
- Order placed → Confirmation message
- Order shipped → Tracking details
- Cart abandoned → Reminder message
- Birthday → Birthday wishes + offer
- Inactive 30 days → Re-engagement

---

## Compliance and Best Practices

### WhatsApp Policies

**Message Guidelines:**
- ✅ Obtain explicit opt-in consent
- ✅ Provide clear opt-out option
- ✅ Send relevant, valuable content
- ✅ Respect message frequency limits
- ✅ Honor unsubscribe requests immediately

**Restricted Content:**
- ❌ Spam or unsolicited messages
- ❌ Misleading information
- ❌ Promotional content without consent
- ❌ Sensitive personal data
- ❌ Illegal or harmful content

**Rate Limits:**
```
Business API Limits:
├── 1,000 messages/day (Tier 1)
├── 10,000 messages/day (Tier 2)
├── 100,000 messages/day (Tier 3)
└── Unlimited (Tier 4 - approved businesses)
```

---

## WhatsApp API Settings

### API Configuration

**Connection Status:**
```
WhatsApp Business API
Status: ✅ Connected
Phone Number: +1 (203) 555-0101
Last Sync: 2 hours ago

[Refresh Connection] [Settings]
```

**API Credentials:**
```
WhatsApp SID: **********
Token: **********
Phone ID: **********
Business Account ID: **********

[Show] [Regenerate]
```

**Webhook Configuration:**
```
Webhook URL:
https://demo.magicproject.ai/api/marketing-bot/whatsapp/1/webhook

Events:
☑ Messages
☑ Message Status
☑ Message Reads
☐ Customer Info Updates

[Test Webhook] [Save]
```

---

## Troubleshooting

### Common Issues

**Messages Not Delivering:**
- **Cause:** Invalid phone number, recipient blocked you, API limit reached
- **Solution:** Verify number format (+country code), check blocked contacts, review API limits

**Contacts Not Syncing:**
- **Cause:** API connection issue, permission problem, cache delay
- **Solution:** Refresh connection, verify API credentials, clear cache and retry

**Template Not Approved:**
- **Cause:** Policy violation, unclear content, missing opt-out
- **Solution:** Review WhatsApp policies, revise template, include unsubscribe option

**Broadcast List Errors:**
- **Cause:** Exceeds 256 limit, contacts don't have your number saved
- **Solution:** Split into multiple lists, ensure contacts saved your number

---

## Next Steps

<div class="grid cards" markdown>

-   :material-bullhorn:{ .lg .middle } __Create Campaign__

    ---

    Broadcast to WhatsApp contacts

    [:octicons-arrow-right-24: Campaigns](campaigns.md)

-   :material-cog:{ .lg .middle } __Bot Settings__

    ---

    Configure WhatsApp API

    [:octicons-arrow-right-24: Settings](settings.md)

-   :material-inbox:{ .lg .middle } __Manage Inbox__

    ---

    View and respond to messages

    [:octicons-arrow-right-24: Inbox](inbox.md)

</div>

---

**Previous:** [← Telegram](telegram.md) | **Next:** [Settings →](settings.md)

---

**Last Updated:** December 2025
