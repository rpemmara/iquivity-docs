# Marketing Bot - Settings

Configure API credentials, webhooks, and integration settings for Telegram and WhatsApp bots.

---

## Overview

The Settings page allows you to configure your Marketing Bot integrations for both Telegram and WhatsApp. Set up API tokens, configure webhooks, and manage environment settings for seamless automated messaging.

!!! info "Secure Configuration"
    All API tokens and sensitive credentials are encrypted and stored securely. Tokens are masked in the interface for security.

---

## Marketing Bot Telegram Settings

### Telegram Bot Configuration

**Access Token:**

```
┌────────────────────────────────────┐
│ Access Token                       │
│                                    │
│ **********                         │
│                                    │
│ [Show] [Regenerate] [Copy]        │
└────────────────────────────────────┘

[Save]
```

**Configuration Steps:**

1. **Obtain Telegram Bot Token:**
   ```
   1. Open Telegram and search for @BotFather
   2. Send /newbot command
   3. Follow prompts to create bot:
      - Enter bot name (e.g., "My Marketing Bot")
      - Enter username (must end in 'bot', e.g., "my_marketing_bot")
   4. BotFather provides API token
   5. Copy the token (format: 1234567890:ABCdefGHIjklMNOpqrsTUVwxyz)
   ```

2. **Configure in Settings:**
   ```
   1. Navigate to Marketing Bot Settings
   2. Locate "Marketing Bot Telegram" section
   3. Paste token in "Access Token" field
   4. Click "Save"
   5. Verify connection status
   ```

**Token Security:**
- Token is masked as `**********` for security
- Click "Show" to reveal token temporarily
- Click "Regenerate" to create new token from BotFather
- Never share your bot token publicly

---

## Marketing Bot WhatsApp Settings

### WhatsApp API Configuration

**WhatsApp SID:**

```
┌────────────────────────────────────┐
│ WhatsApp SID                       │
│                                    │
│ **********                         │
│                                    │
│ [Show] [Copy]                      │
└────────────────────────────────────┘
```

**WhatsApp Token:**

```
┌────────────────────────────────────┐
│ WhatsApp Token                     │
│                                    │
│ **********                         │
│                                    │
│ [Show] [Regenerate] [Copy]        │
└────────────────────────────────────┘
```

**WhatsApp Phone:**

```
┌────────────────────────────────────┐
│ WhatsApp Phone                     │
│                                    │
│ **********                         │
│                                    │
│ [Show] [Edit]                      │
└────────────────────────────────────┘
```

**WhatsApp Sandbox Phone:**

```
┌────────────────────────────────────┐
│ WhatsApp Sandbox Phone             │
│                                    │
│ **********                         │
│                                    │
│ [Show] [Edit]                      │
└────────────────────────────────────┘
```

---

## WhatsApp Configuration Steps

### Setting up WhatsApp Business API

**Step 1: Get WhatsApp Business API Access**

```
Option 1: Twilio (Recommended for testing)
1. Create account at twilio.com
2. Navigate to WhatsApp section
3. Get sandbox credentials for testing
4. Upgrade to production when ready

Option 2: Facebook Business Manager
1. Create Facebook Business Manager account
2. Apply for WhatsApp Business API access
3. Wait for approval (may take several days)
4. Configure business profile
5. Get API credentials

Option 3: Third-party Provider
1. Choose WhatsApp BSP (Business Solution Provider)
2. Sign up and verify business
3. Complete onboarding process
4. Receive API credentials
```

**Step 2: Configure Credentials**

```
1. WhatsApp SID:
   - Account identifier from provider
   - Paste in "WhatsApp SID" field

2. WhatsApp Token:
   - API authentication token
   - Paste in "WhatsApp Token" field

3. WhatsApp Phone:
   - Your business phone number
   - Format: +[country code][number]
   - Example: +12035550101

4. WhatsApp Sandbox Phone:
   - Testing/development number
   - Used for sandbox environment
   - Format: +[country code][number]
```

---

## Environment Settings

### Environment Selection

**Environment Dropdown:**

```
┌────────────────────────────────────┐
│ Environment                        │
│                                    │
│ [PRODUCTION ▼]                    │
│   - PRODUCTION                     │
│   - SANDBOX                        │
│   - DEVELOPMENT                    │
│                                    │
└────────────────────────────────────┘
```

**Environment Types:**

**PRODUCTION:**
- Live environment for actual customers
- Real phone numbers
- Charges apply for messages
- Requires approved Business API
- No testing prefix needed

**SANDBOX:**
- Testing environment
- Use sandbox phone numbers
- Free message sending
- Test bot functionality
- No real customer impact

**DEVELOPMENT:**
- Local development environment
- Internal testing only
- Mock responses available
- Debug mode enabled
- Development webhooks

---

## Webhook Configuration

### Telegram Webhook

**Webhook URL:**

```
Telegram Webhook URL:
https://demo.magicproject.ai/api/marketing-bot/telegram/webhook

Status: ✅ Active
Last Event: 2 minutes ago
Events Received (24h): 1,247

[Test Webhook] [View Logs] [Refresh]
```

**Webhook Events:**
```
Subscribed Events:
☑ Message Received
☑ Message Sent
☑ Message Delivered
☑ Message Read
☑ New Member Joined
☑ Member Left
☐ Group Created
☐ Group Settings Changed
```

---

### WhatsApp Webhook

**Webhook URL:**

```
WhatsApp Webhook URL:
https://demo.magicproject.ai/api/marketing-bot/whatsapp/1/webhook

Status: ✅ Active
Last Event: 1 minute ago
Events Received (24h): 856

[Test Webhook] [View Logs] [Refresh]
```

**Webhook Events:**
```
Subscribed Events:
☑ Message Received
☑ Message Status Update
☑ Message Read Receipt
☑ Delivery Notification
☐ Customer Profile Update
☐ Template Status Change
```

**Webhook Configuration:**
```
1. Copy webhook URL from settings
2. Navigate to your provider dashboard:
   - Twilio: Console > WhatsApp > Sandbox/Production
   - Facebook: WhatsApp Manager > Webhooks
3. Paste webhook URL
4. Subscribe to events
5. Test webhook connection
6. Save configuration
```

---

## Testing Configuration

### Verify Bot Setup

**Test Telegram Bot:**

```
1. Open Telegram app
2. Search for your bot (@your_bot_username)
3. Send /start command
4. Bot should respond with welcome message
5. Check Settings page for webhook activity
6. Verify events appear in logs
```

**Test WhatsApp Bot:**

```
Sandbox Testing:
1. Join sandbox using provided number
2. Send required code message
3. Send test message to bot
4. Bot should respond or log message
5. Check webhook status in Settings
6. Verify message delivery

Production Testing:
1. Send message from registered business number
2. Use approved message template
3. Verify delivery to customer
4. Check webhook events
5. Review analytics
```

---

## Connection Status

### Monitor Integration Health

**Status Indicators:**

**Connected (✅):**
- Green checkmark
- All credentials valid
- Webhook active
- Receiving events
- Ready for use

**Disconnected (❌):**
- Red X mark
- Invalid credentials
- Webhook inactive
- Not receiving events
- Requires attention

**Warning (⚠️):**
- Yellow warning icon
- Partial configuration
- Some events failing
- Check logs
- May need update

---

## Security Best Practices

### Protecting Your Credentials

**Token Management:**
- ✅ Never share API tokens publicly
- ✅ Rotate tokens regularly (every 90 days)
- ✅ Use environment variables
- ✅ Restrict token permissions
- ✅ Monitor token usage

**Access Control:**
- 🔒 Limit team member access to settings
- 🔐 Use strong passwords
- 👥 Enable two-factor authentication
- 📝 Audit access logs
- ⏰ Review permissions regularly

**Webhook Security:**
- 🔑 Use HTTPS only
- ✅ Validate webhook signatures
- 🛡️ Implement rate limiting
- 📊 Monitor for suspicious activity
- 🚨 Set up alerts for failures

---

## Troubleshooting

### Common Configuration Issues

**Telegram Bot Not Responding:**
- **Cause:** Invalid token, webhook not configured, bot not started
- **Solution:**
  - Verify token from BotFather
  - Check webhook URL is correct
  - Send /start to bot in Telegram
  - Review webhook logs

**WhatsApp Messages Failing:**
- **Cause:** Invalid credentials, number not verified, template not approved
- **Solution:**
  - Verify all API credentials
  - Check phone number format
  - Ensure templates are approved
  - Review rate limits

**Webhook Not Receiving Events:**
- **Cause:** Incorrect URL, HTTPS required, firewall blocking
- **Solution:**
  - Verify webhook URL format
  - Ensure HTTPS (not HTTP)
  - Check server firewall rules
  - Test webhook connectivity

**Environment Mismatch:**
- **Cause:** Using production credentials in sandbox
- **Solution:**
  - Match environment to credentials
  - Use sandbox phone for sandbox env
  - Switch environment dropdown
  - Save and test again

---

## Advanced Configuration

### Custom Webhook Settings

**Webhook Retry Policy:**
```
Failed Event Handling:
├── Retry Count: 3 attempts
├── Retry Delay: Exponential backoff
├── Max Delay: 5 minutes
└── Failure Action: Log and alert
```

**Rate Limiting:**
```
API Rate Limits:
├── Requests per second: 50
├── Requests per minute: 1,000
├── Daily message limit: Based on tier
└── Burst allowance: 100 messages
```

**Logging Configuration:**
```
Log Settings:
☑ Log all webhook events
☑ Log API requests
☑ Log errors only
☐ Debug mode (verbose logging)
☐ Log message content (privacy concern)

Retention: 30 days
```

---

## API Documentation

### Developer Resources

**Telegram Bot API:**
- Documentation: https://core.telegram.org/bots/api
- Bot features: Commands, inline keyboards, media
- Rate limits: 30 messages/second per chat

**WhatsApp Business API:**
- Documentation: https://developers.facebook.com/docs/whatsapp
- Message templates: Required for business-initiated messages
- Rate limits: Tiered based on quality rating

---

## Backup and Export

### Configuration Backup

**Export Settings:**
```
1. Click "Export Configuration"
2. Save JSON file securely
3. Store in secure location
4. Include in backup routine
5. Use for disaster recovery
```

**Import Settings:**
```
1. Click "Import Configuration"
2. Select JSON backup file
3. Review imported settings
4. Save configuration
5. Test connections
```

---

## Next Steps

<div class="grid cards" markdown>

-   :fontawesome-brands-telegram:{ .lg .middle } __Telegram Setup__

    ---

    Configure Telegram bot and groups

    [:octicons-arrow-right-24: Telegram](telegram.md)

-   :fontawesome-brands-whatsapp:{ .lg .middle } __WhatsApp Setup__

    ---

    Manage WhatsApp contacts and campaigns

    [:octicons-arrow-right-24: WhatsApp](whatsapp.md)

-   :material-bullhorn:{ .lg .middle } __Create Campaigns__

    ---

    Start broadcasting messages

    [:octicons-arrow-right-24: Campaigns](campaigns.md)

</div>

---

**Previous:** [← WhatsApp](whatsapp.md) | **Up:** [Dashboard](dashboard.md)

---

**Last Updated:** December 2025
