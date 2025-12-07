# AI Bot Contacts

Manage your chatbot contacts and view their interaction history with your AI Bots.

---

## Overview

AI Bot Contacts is a centralized contact management system that captures and stores information about visitors who interact with your AI Bots. This feature helps you track leads, manage customer relationships, and view conversation history.

---

## Accessing AI Bot Contacts

**Navigate to Contacts:**

1. From the main dashboard, locate **"AI Bot Contacts"** in the left-hand navigation
2. Click to open the Contacts management page

**Dashboard View:**

The Contacts page displays a table with all captured contacts:

| Column | Description |
|--------|-------------|
| **ID** | Unique identifier for each contact |
| **Name** | Contact's name (if provided) |
| **Email** | Contact's email address |
| **Phone** | Contact's phone number (if provided) |
| **Channel** | Source channel (frame, livechat, telegram, messenger, whatsapp) |
| **Created At** | Date and time contact was first captured |
| **Actions** | Edit (✏️) and Delete (✖) options |

**Example Contacts:**

```
ID  NAME              EMAIL                    PHONE           CHANNEL  CREATED AT
1   Olivia Bennett    olivia@lumoco.dev        +482-719-364    frame    22.8.2025 05:02:29
2   Mason Clark       mason@northpeak.co       +935-204-188    frame    22.8.2025 05:03:28
3   Harper Mitchell   harper@sparkwave.app     +261-853-047    frame    22.8.2025 05:03:35
```

---

## How Contacts Are Captured

### Automatic Contact Collection

Contacts are automatically created when visitors interact with your AI Bot and provide their information:

**Contact Collection Methods:**

**1. Email Collection Feature**
- When "Email Collect" is enabled in bot settings
- Bot prompts users for email during conversation
- Email automatically saved to Contacts

**2. Contact Form Submission**
- When "Contact Us" feature is enabled
- Users fill out contact form in chat
- Information saved to Contacts database

**3. Channel Integration**
- Facebook Messenger: Profile name and ID
- Telegram: Username and ID
- WhatsApp: Phone number and name
- Website: Provided name and email

**4. Conversation Initiation**
- User starts chat on any channel
- Basic contact record created
- Additional info added as conversation progresses

### Contact Information Fields

**Standard Fields:**

| Field | Source | Required |
|-------|--------|----------|
| **Name** | User provides or channel profile | Optional |
| **Email** | User provides | Optional |
| **Phone** | User provides or WhatsApp | Optional |
| **Channel** | Automatically detected | Yes |
| **Created At** | System timestamp | Yes |

---

## Viewing Contact Details

### Contact Information

**Click on any contact** to view detailed information:

**Contact Profile:**
```
Name: Olivia Bennett
Email: olivia@lumoco.dev
Phone: +482-719-364
Channel: frame (Website widget)
First Contact: 22.8.2025 05:02:29
Last Activity: 22.8.2025 05:15:42
```

### Conversation History

**View all conversations** this contact has had with your AI Bots:

**Conversation Log:**
```
Conversation #1 - 22.8.2025 05:02:29
Channel: Website Widget
Duration: 5 minutes
Messages: 12
Status: Closed

Conversation #2 - 22.8.2025 05:15:12
Channel: Website Widget
Duration: 3 minutes
Messages: 8
Status: Closed
```

**Click on a conversation** to view full chat transcript.

---

## Managing Contacts

### Editing Contact Information

**To Update Contact Details:**

1. Locate the contact in the table
2. Click the **Edit icon (✏️)** in the Actions column
3. Update the following fields:
   - Name
   - Email
   - Phone number
   - Notes (if available)
4. Click **"Save"** to update

**When to Edit:**
- Correct spelling errors in name
- Update email address
- Add missing phone number
- Merge duplicate entries
- Add internal notes

### Deleting Contacts

**To Remove a Contact:**

1. Locate the contact in the table
2. Click the **Delete icon (✖)** in the Actions column
3. Confirm deletion when prompted

!!! warning "Deletion Warning"
    Deleting a contact removes all associated conversation history. This action cannot be undone.

**When to Delete:**
- Duplicate contact entries
- Test contacts from bot testing
- Spam or invalid contacts
- Upon user's data deletion request
- GDPR/privacy compliance

---

## Filtering and Searching Contacts

### Search by Channel

**Filter contacts by source channel:**

- **All Channels** - Show all contacts
- **frame** - Website widget contacts
- **livechat** - Live chat contacts
- **telegram** - Telegram bot contacts
- **messenger** - Facebook Messenger contacts
- **whatsapp** - WhatsApp contacts

### Search by Date

**Filter by creation date:**
- Today
- Last 7 days
- Last 30 days
- Custom date range

### Search by Name/Email

**Use search box to find contacts by:**
- Name
- Email address
- Phone number

---

## Using Contact Data

### Lead Management

**Track and Qualify Leads:**

**Lead Status Indicators:**
```
🔵 New Contact
├─ Just added to system
├─ First conversation
└─ Needs follow-up

🟢 Active Lead
├─ Multiple conversations
├─ Showing interest
└─ Engaged with content

🟡 Follow-up Needed
├─ Hasn't responded recently
├─ Incomplete information
└─ Schedule outreach

⚪ Archived/Inactive
├─ No recent activity
├─ Opted out
└─ Moved to CRM
```

### Export Contacts

**Export contact data for:**
- CRM integration
- Email marketing campaigns
- Sales team follow-up
- Analytics and reporting

**Export Options:**
- CSV format
- Excel spreadsheet
- JSON data
- Filtered exports (by channel, date, etc.)

### Integration with CRM

**Sync contacts to external CRM:**
- Salesforce
- HubSpot
- Zoho CRM
- Custom integrations via API

---

## Contact Privacy and Compliance

### Data Protection

**GDPR Compliance:**
- Contacts can request data deletion
- Export contact data upon request
- Clear consent for data collection
- Secure data storage

**Privacy Best Practices:**
- ✅ Only collect necessary information
- ✅ Clearly state data usage policies
- ✅ Provide opt-out options
- ✅ Secure storage and transmission
- ✅ Regular data audits
- ✅ Honor deletion requests promptly

### Data Retention

**Retention Policies:**

```
Active Contacts
├─ Retain indefinitely while active
├─ Regular conversation activity
└─ Ongoing relationship

Inactive Contacts
├─ Review after 12 months of inactivity
├─ Option to archive or delete
└─ Comply with data retention laws

Deleted Contacts
├─ Permanent deletion upon request
├─ 30-day grace period (optional)
└─ Remove all associated data
```

---

## Contact Analytics

### Contact Insights

**Track key metrics:**

**Total Contacts:**
```
Total Contacts: 1,247
├─ New this month: 89
├─ Active conversations: 34
└─ Awaiting follow-up: 12
```

**Channel Breakdown:**
```
Website Widget: 856 contacts (69%)
Facebook Messenger: 234 contacts (19%)
Telegram: 98 contacts (8%)
WhatsApp: 59 contacts (5%)
```

**Engagement Metrics:**
```
Avg. Conversations per Contact: 2.3
Avg. Response Time: 3.5 minutes
Conversion Rate: 18%
Repeat Visitors: 34%
```

---

## Best Practices

### Contact Management Tips

**1. Regular Maintenance**
- Review contacts weekly
- Remove duplicates monthly
- Archive inactive contacts quarterly
- Export backups regularly

**2. Organize Contacts**
- Use consistent naming conventions
- Add tags or categories (if available)
- Note important details in contact records
- Link related conversations

**3. Follow-up Strategy**
```
Immediate Follow-up (within 24 hours):
└─ High-intent leads (pricing inquiries, demo requests)

Short-term Follow-up (within 7 days):
└─ General inquiries, product questions

Long-term Nurture (monthly):
└─ Newsletter subscribers, early-stage interest
```

**4. Data Quality**
- Verify email addresses
- Standardize phone number formats
- Complete partial records when possible
- Merge duplicate contacts

### Lead Scoring

**Prioritize contacts based on engagement:**

**Hot Leads (High Priority):**
- Multiple conversations
- Asked about pricing/plans
- Requested demo or trial
- Engaged recently (< 7 days)

**Warm Leads (Medium Priority):**
- 1-2 conversations
- Product interest shown
- Some engagement (7-30 days ago)
- Information gathering stage

**Cold Leads (Low Priority):**
- Single conversation
- General questions only
- No recent activity (> 30 days)
- Low engagement

---

## Use Cases

### Sales Lead Tracking

**Track potential customers:**

```
Contact: Sarah Johnson
Email: sarah@techstartup.com
Channel: Website Widget
Conversations: 3

Timeline:
├─ Day 1: Asked about Pro plan features
├─ Day 3: Requested pricing details
└─ Day 5: Inquired about enterprise options

Next Action: Follow up with enterprise demo offer
Priority: High
```

### Customer Support History

**View support interaction history:**

```
Contact: Michael Chen
Email: michael@company.com
Phone: +1-555-0123
Channel: Live Chat

Support History:
├─ Issue #1: Password reset (Resolved)
├─ Issue #2: Billing question (Resolved)
└─ Issue #3: Feature request (Forwarded to product team)

Customer Satisfaction: 4.5/5
```

### Marketing Campaign Tracking

**Identify engaged contacts for campaigns:**

```
Segment: Active Newsletter Subscribers
Criteria:
├─ Engaged in last 30 days
├─ Email provided
├─ Opted in for updates
└─ No unsubscribe requests

Total Contacts: 456
Campaign: New Feature Announcement
```

---

## Troubleshooting

### Common Issues

**Problem: Contact Not Appearing**
- **Cause:** Email collection not enabled in bot settings
- **Solution:** Enable "Email Collect" feature in bot customization

**Problem: Duplicate Contacts**
- **Cause:** Same person chatting from different channels
- **Solution:** Manually merge duplicate contact records

**Problem: Missing Contact Information**
- **Cause:** User didn't provide all details
- **Solution:** Enable progressive profiling to collect info over time

**Problem: Cannot Delete Contact**
- **Cause:** Contact has active conversations
- **Solution:** Close all conversations first, then delete

---

## API Access

### Programmatic Contact Management

**Access contacts via API:**

```json
GET /api/v1/contacts

Response:
{
  "contacts": [
    {
      "id": 1,
      "name": "Olivia Bennett",
      "email": "olivia@lumoco.dev",
      "phone": "+482-719-364",
      "channel": "frame",
      "created_at": "2025-08-22T05:02:29Z"
    }
  ],
  "total": 1247,
  "page": 1
}
```

**Use Cases for API:**
- Sync to external CRM
- Custom reporting dashboards
- Automated follow-up workflows
- Data backup and export

---

## Additional Resources

<div class="grid cards" markdown>

-   :material-robot:{ .lg .middle } __AI Bot Overview__

    ---

    Learn about AI Bot features

    [:octicons-arrow-right-24: Overview](overview.md)

-   :material-inbox:{ .lg .middle } __CRM Inbox__

    ---

    Manage conversations and replies

    [:octicons-arrow-right-24: Deployment Guide](deployment.md#human-agent-integration)

</div>

---

**Previous:** [← AI Bot Knowledge Base](knowledge-base.md) | **Up:** [AI Bot Overview](overview.md)

---

**Last Updated:** December 2025
