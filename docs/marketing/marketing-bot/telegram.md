# Marketing Bot - Telegram

Manage Telegram groups, subscribers, and broadcast campaigns for automated messaging on Telegram.

---

## Overview

The Telegram integration allows you to manage groups, track subscribers, and broadcast messages to your Telegram audience. Connect your Telegram bot, organize groups, and automate your messaging workflows.

!!! info "Telegram Groups"
    Manage multiple Telegram groups and broadcast to thousands of subscribers simultaneously.

---

## Telegram Groups

### Group Management

**Groups List View:**

| ID | Name | Action |
|----|------|--------|
| 1 | Tech Lovers | ✕ |
| 2 | Marketing Gurus | ✕ |
| 3 | Startup Founders | ✕ |
| 4 | Fitness Enthusiasts | ✕ |
| 5 | Book Club | ✕ |
| 6 | Crypto Traders | ✕ |

**Group Information:**
- Group ID and name
- Member count
- Creation date
- Activity status
- Bot permissions

**Group Actions:**
- **Remove (✕)**: Disconnect group from bot
- **View Members**: See subscriber list
- **Send Message**: Broadcast to group
- **Group Settings**: Configure options
- **Export Data**: Download member list

---

## Adding Telegram Groups

### Connect New Group

**Step 1: Add Bot to Group**
```
1. Open Telegram group
2. Click group info
3. Select "Add Members"
4. Search for your bot (@your_bot_name)
5. Add bot to group
6. Grant admin permissions
```

**Step 2: Sync with Platform**
```
1. Navigate to Telegram Groups page
2. Click "+ Add Group" button
3. Group appears in list automatically
4. Verify bot permissions
5. Test message sending
```

**Required Permissions:**
- Send messages
- Delete messages (optional)
- Pin messages (optional)
- Invite users (optional)
- Manage group (recommended)

---

## Group Subscribers

### Subscriber Management

**Subscribers List View:**

| ID | Name | Username | Action |
|----|------|----------|--------|
| 1 | John Doe | @john_doe | ✕ |
| 2 | Jane Smith | @jane_smith | ✕ |
| 3 | Mike Johnson | @mike_johnson | ✕ |
| 4 | Emily Davis | @emily_davis | ✕ |
| 5 | Robert Wilson | @robert_wilson | ✕ |
| 6 | Laura Brown | @laura_brown | ✕ |
| 7 | Daniel Miller | @daniel_miller | ✕ |

**Subscriber Details:**
- Telegram user ID
- Display name
- Username (if available)
- Join date
- Activity status
- Message count

**Subscriber Actions:**
- **Remove (✕)**: Remove from group
- **Block**: Prevent from rejoining
- **Message**: Send direct message
- **View History**: See message activity
- **Add to Segment**: Organize subscribers

---

## Broadcasting to Groups

### Send Messages to Groups

**Broadcast Options:**

**Select Target Groups:**
```
☐ Tech Lovers (2,450 members)
☐ Marketing Gurus (1,823 members)
☐ Startup Founders (945 members)
☐ Fitness Enthusiasts (3,102 members)
☐ Book Club (567 members)
☐ Crypto Traders (4,891 members)

Total Reach: [Selected groups member count]
```

**Message Types:**
- Text messages
- Photos and videos
- Documents and files
- Polls
- Stickers
- Location
- Contact cards

**Message Features:**
- Markdown formatting
- HTML formatting
- Inline buttons
- Reply keyboards
- Link previews
- Silent messages (no notification)

---

## Bot Commands

### Telegram Bot Commands

**Default Commands:**
```
/start - Initialize bot conversation
/help - Show available commands
/subscribe - Subscribe to updates
/unsubscribe - Unsubscribe from updates
/status - Check subscription status
/info - Bot and group information
```

**Custom Commands:**
```
Add custom commands:
/offer - Show current offers
/support - Contact support
/faq - Frequently asked questions
/track - Track order status
/feedback - Submit feedback
```

**Command Configuration:**
```
1. Navigate to Settings
2. Select "Bot Commands"
3. Add new command
4. Define response
5. Set permissions
6. Save and test
```

---

## Telegram Campaign Integration

### Create Telegram Campaigns

**From Groups Page:**
```
1. Select target groups
2. Click "Create Campaign"
3. Compose message
4. Schedule or send immediately
5. Track delivery and engagement
```

**Campaign Features:**
- Multi-group broadcasting
- Scheduled sends
- Message templates
- Media attachments
- Analytics tracking
- Delivery reports

---

## Group Analytics

### Performance Metrics

**Group Statistics:**
```
Group: Tech Lovers
───────────────────────────
Members:         2,450
Active Members:  1,876 (76.6%)
Messages/Day:    342
Engagement Rate: 15.2%
Growth (30d):    +145 members
```

**Engagement Metrics:**
- Message views
- Reactions
- Replies
- Shares/Forwards
- Bot interactions
- Command usage

---

## Group Moderation

### Manage Group Content

**Moderation Tools:**
- Delete messages
- Ban users
- Restrict users
- Pin important messages
- Set slow mode
- Filter content

**Auto-Moderation:**
```
Configure auto-moderation:
├── Spam filtering
├── Link blocking
├── Profanity filter
├── Media restrictions
└── Join/Leave messages
```

---

## Telegram Bot Settings

### Bot Configuration

**Access Token:**
```
Bot Token: **********
Status: Connected
Last Update: 2 hours ago

[Refresh Token] [Regenerate]
```

**Bot Information:**
```
Bot Name: @your_marketing_bot
Bot ID: 1234567890
Created: Jan 15, 2025
Status: Active
```

**Webhook Configuration:**
```
Webhook URL: https://demo.magicproject.ai/api/marketing-bot/telegram/webhook
Status: Active
Last Event: 2 minutes ago

[Test Webhook] [Refresh]
```

---

## Best Practices

### Telegram Group Management

**Content Strategy:**
- ✅ Post valuable content regularly
- ✅ Engage with members
- ✅ Use polls and quizzes
- ✅ Share exclusive offers
- ✅ Respond to questions promptly

**Group Growth:**
- 📢 Promote group in other channels
- 🎁 Offer incentives for joining
- 🤝 Collaborate with other groups
- 📊 Track growth metrics
- 🔄 Consistent posting schedule

**Engagement Tips:**
- 💬 Encourage discussions
- 🎯 Target relevant content
- 📸 Use visual content
- 🎮 Interactive elements
- ⏰ Post at optimal times

---

## Troubleshooting

### Common Issues

**Bot Not Responding:**
- **Cause:** Invalid token, bot not admin, API issues
- **Solution:** Verify token, check admin rights, test webhook

**Messages Not Sending:**
- **Cause:** Bot kicked from group, rate limit, permissions
- **Solution:** Re-add bot, wait and retry, grant permissions

**Subscribers Not Syncing:**
- **Cause:** Cache delay, API timeout, permissions
- **Solution:** Refresh page, check connection, verify bot access

---

## Next Steps

<div class="grid cards" markdown>

-   :fontawesome-brands-whatsapp:{ .lg .middle } __WhatsApp Setup__

    ---

    Configure WhatsApp integration

    [:octicons-arrow-right-24: WhatsApp](whatsapp.md)

-   :material-bullhorn:{ .lg .middle } __Create Campaign__

    ---

    Broadcast to Telegram groups

    [:octicons-arrow-right-24: Campaigns](campaigns.md)

-   :material-cog:{ .lg .middle } __Bot Settings__

    ---

    Configure Telegram bot

    [:octicons-arrow-right-24: Settings](settings.md)

</div>

---

**Previous:** [← Campaigns](campaigns.md) | **Next:** [WhatsApp →](whatsapp.md)

---

**Last Updated:** December 2025
