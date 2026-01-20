# Profile Settings

Manage your personal information, preferences, and account settings.

## Accessing Profile Settings Test

Navigate to **Settings** → **Profile** from the dashboard.

## Personal Information

### Basic Details

Update your account information:

```
┌─────────────────────────────────────┐
│ Profile Photo                       │
│  ┌──────┐                          │
│  │ [JD] │  [Upload Photo]          │
│  └──────┘  [Remove Photo]          │
│                                     │
│ Full Name                           │
│ [John Doe________________]          │
│                                     │
│ Email Address                       │
│ [john.doe@example.com___] Verified │
│ [Change Email]                      │
│                                     │
│ Phone Number (optional)             │
│ [+1 (555) 123-4567______]          │
│ [Verify Phone]                      │
│                                     │
│ Job Title                           │
│ [Marketing Manager______]           │
│                                     │
│ Company/Organization                │
│ [Acme Corporation_______]           │
│                                     │
│ Bio/Description (optional)          │
│ [________________________]          │
│ [________________________]          │
│ [________________________]          │
│                                     │
│ [Save Changes]  [Cancel]            │
└─────────────────────────────────────┘
```

### Profile Photo

**Upload Requirements:**
- Supported formats: JPG, PNG, GIF
- Maximum size: 5 MB
- Recommended: Square image, 400x400px or larger
- Displays in: Dashboard, comments, team views, chat

**Photo Options:**
- Upload custom photo
- Use initials avatar (default)
- Remove current photo

### Email Management

**Primary Email:**
- Used for login
- Receives all notifications
- Cannot be removed

**Changing Email:**
1. Click **"Change Email"**
2. Enter new email address
3. Enter current password
4. Verify new email (check inbox)
5. Confirm change

!!! warning "Email Verification Required"
    You must verify your new email address before it becomes active. You'll continue using your old email until verification is complete.

**Additional Emails:**
- Add backup email addresses
- Receive notifications at multiple addresses
- Use for login (optional)

### Phone Verification

**Enable Phone Verification:**
1. Enter phone number
2. Click **"Verify Phone"**
3. Receive SMS code
4. Enter code to verify

**Benefits:**
- Two-factor authentication via SMS
- Account recovery option
- Phone support (premium plans)
- Important alerts via SMS

## Regional Settings

### Timezone

**Configure Your Timezone:**

```
Timezone: [EST (UTC-5) ▼]

Common timezones:
• EST (UTC-5) - Eastern Standard Time
• PST (UTC-8) - Pacific Standard Time
• GMT (UTC+0) - Greenwich Mean Time
• CET (UTC+1) - Central European Time
• JST (UTC+9) - Japan Standard Time

☑ Automatically detect timezone
☐ Use 24-hour time format
```

**Impact:**
- Timestamp displays
- Scheduled reports
- Chatbot operating hours
- Activity logs
- Analytics reports

### Language Preference

**Interface Language:**

```
Display Language: [English (US) ▼]

Available Languages:
• English (US)
• English (UK)
• Español
• Français
• Deutsch
• Italiano
• Português
• 日本語
• 中文
• 한국어
• + 40 more languages
```

**Content Language:**
```
Default Content Language: [English ▼]

This sets the default language for:
• AI-generated content
• Templates
• Chatbot responses
```

### Date Format

```
Date Format: [MM/DD/YYYY ▼]

Options:
• MM/DD/YYYY (12/02/2024)
• DD/MM/YYYY (02/12/2024)
• YYYY-MM-DD (2024-12-02)
• DD Month YYYY (02 December 2024)

Time Format:
● 12-hour (3:30 PM)
○ 24-hour (15:30)
```

## Account Preferences

### Content Preferences

**Default Settings for Content Generation:**

```
┌─────────────────────────────────────┐
│ Default Content Tone                │
│ ● Professional                      │
│ ○ Casual                           │
│ ○ Friendly                         │
│ ○ Formal                           │
│                                     │
│ Preferred AI Models                 │
│ Text: [GPT-4 ▼]                    │
│ Images: [DALL-E 3 ▼]               │
│ Video: [Standard ▼]                │
│                                     │
│ Auto-save Frequency                 │
│ [Every 30 seconds ▼]               │
│                                     │
│ Default Export Format               │
│ Documents: [PDF ▼]                 │
│ Spreadsheets: [XLSX ▼]             │
│                                     │
│ Content Organization                │
│ ☑ Auto-tag generated content        │
│ ☑ Create dated folders              │
│ ☐ Use project-based organization    │
└─────────────────────────────────────┘
```

### Dashboard Preferences

**Customize Dashboard Experience:**

```
Dashboard Layout:
○ Compact view
● Standard view
○ Expanded view

Default Landing Page:
[Dashboard ▼]
• Dashboard
• AI Writer
• Recent Files
• Analytics

Show on Dashboard:
☑ Quick Actions
☑ Recent Activity
☑ Usage Statistics
☑ Team Activity
☐ Tips and Tutorials
☑ What's New
```

### Editor Preferences

**Text Editor Settings:**

```
Editor Mode:
● Rich text (visual)
○ Markdown
○ HTML

Formatting:
Font: [Inter ▼]
Size: [14px ▼]

☑ Show line numbers
☑ Enable spell check
☑ Enable grammar check
☑ Auto-correct
☐ Show word count in real-time

Keyboard Shortcuts:
● Enabled (standard)
○ Enabled (custom)
○ Disabled
```

## Notification Preferences

Control how and when you receive notifications.

### Email Notifications

```
┌─────────────────────────────────────┐
│ Email Notification Settings         │
├─────────────────────────────────────┤
│                                     │
│ Account Activity                    │
│ ☑ Login from new device             │
│ ☑ Password changed                  │
│ ☑ Email changed                     │
│ ☑ Security alerts                   │
│                                     │
│ Usage Alerts                        │
│ ☑ Credit balance low (< 10%)        │
│ ☑ Storage nearly full (> 90%)       │
│ ☑ Monthly usage summary             │
│ ☐ Daily activity digest             │
│                                     │
│ Collaboration                       │
│ ☑ @mentions in comments             │
│ ☑ Document shared with me           │
│ ☑ Comment replies                   │
│ ☐ All team activity                 │
│                                     │
│ Chatbot Notifications               │
│ ☑ Handoff requests                  │
│ ☑ Low satisfaction ratings          │
│ ☐ Every conversation                │
│ ☑ Weekly performance report         │
│                                     │
│ Marketing & Updates                 │
│ ☑ Product updates                   │
│ ☑ Feature announcements             │
│ ☐ Tips and best practices           │
│ ☐ Promotional offers                │
│ ☐ Partner offers                    │
│                                     │
│ Digest Frequency                    │
│ ● Real-time                         │
│ ○ Hourly digest                     │
│ ○ Daily digest                      │
│ ○ Weekly digest                     │
│                                     │
│ [Unsubscribe from All] [Save]       │
└─────────────────────────────────────┘
```

### Browser Notifications

```
In-App Notifications:
☑ Enable browser notifications
☑ Play sound for notifications
☑ Show desktop notifications

Show Notifications For:
☑ @mentions
☑ Comments
☑ Shares
☑ Team activity
☐ All updates
```

### Mobile Push Notifications

**Mobile App Settings** (if applicable):

```
Push Notifications:
☑ Enable push notifications

Priority Notifications:
☑ Security alerts
☑ Handoff requests
☑ Direct mentions
☑ Important updates

Quiet Hours:
☑ Enable quiet hours
From: [10:00 PM ▼]
To: [7:00 AM ▼]
```

## Privacy Settings

### Data & Privacy

**Control Your Data:**

```
┌─────────────────────────────────────┐
│ Privacy & Data Controls             │
├─────────────────────────────────────┤
│                                     │
│ Profile Visibility                  │
│ ● Team members only                 │
│ ○ Anyone in organization            │
│ ○ Public profile                    │
│                                     │
│ Activity Visibility                 │
│ ☑ Show in team activity feed        │
│ ☐ Show what I'm working on          │
│ ☑ Show online status                │
│                                     │
│ Data Collection                     │
│ ☑ Usage analytics                   │
│ ☑ Performance metrics               │
│ ☐ Marketing analytics               │
│ ☑ Error reporting                   │
│                                     │
│ Third-Party Integrations            │
│ ☑ Allow third-party integrations    │
│ ○ Require approval for each         │
│ ○ Block all integrations            │
│                                     │
│ [Manage Connected Apps]             │
└─────────────────────────────────────┘
```

### Data Retention

```
Content Retention:
● Keep all content indefinitely
○ Auto-delete after [90] days
○ Custom retention policy

Trash Retention:
Deleted items kept for: [30 days ▼]
• 7 days
• 30 days (recommended)
• 60 days
• 90 days
• Never delete automatically
```

### Data Export

**Download Your Data:**

```
Export Account Data

What to include:
☑ Profile information
☑ Generated content
☑ Uploaded files
☑ Templates
☑ Chatbot data
☑ Conversation history
☑ Analytics data
☐ Account activity logs

Format:
● JSON (machine-readable)
○ ZIP with files + CSV
○ Both formats

[Request Export]

Export History:
• export_2024-12-01.zip (2.4 GB) [Download]
• export_2024-11-01.zip (2.1 GB) [Download]

Note: Exports are available for 7 days
```

## Connected Accounts

### Third-Party Integrations

**Manage Connected Services:**

```
┌─────────────────────────────────────┐
│ Connected Accounts                  │
├─────────────────────────────────────┤
│                                     │
│ 🔵 Google Drive          Connected  │
│ Access: Read/Write files            │
│ Connected: 2 months ago             │
│ [Disconnect] [Manage Permissions]   │
│                                     │
│ 📘 Dropbox              Connected  │
│ Access: Read/Write files            │
│ Connected: 1 month ago              │
│ [Disconnect] [Manage Permissions]   │
│                                     │
│ 💬 Slack                Not Connected│
│ [Connect Slack]                     │
│                                     │
│ 📝 WordPress            Not Connected│
│ [Connect WordPress]                 │
│                                     │
└─────────────────────────────────────┘

[Connect More Services]
```

**Available Integrations:**
- Cloud Storage (Google Drive, Dropbox, OneDrive)
- Communication (Slack, Microsoft Teams, Discord)
- CMS (WordPress, Webflow, Squarespace)
- Automation (Zapier, Make)
- Development (GitHub, GitLab)

## Account Status

### Subscription Information

```
╔════════════════════════════════════╗
║ Current Plan: Professional         ║
╠════════════════════════════════════╣
║ Billing Cycle: Monthly             ║
║ Next Billing Date: Jan 2, 2025     ║
║ Amount: $99.00/month               ║
║                                    ║
║ [View Billing Details]             ║
║ [Upgrade Plan] [Change Plan]       ║
╚════════════════════════════════════╝
```

### Usage Statistics

```
This Month's Usage:

Credits: 4,250 / 10,000 (42%)
████████░░░░░░░░░░

Storage: 45 GB / 100 GB (45%)
█████████░░░░░░░░░░░

API Calls: 342 / 1,000 (34%)
███████░░░░░░░░░░░░░

Team Members: 5 / 5 (100%)
████████████████████

[View Detailed Usage]
```

## Account Actions

### Danger Zone

```
⚠️  Dangerous Actions

[Change Password]
Update your account password

[Delete Account]
Permanently delete your account and all data
⚠️  This action cannot be undone!

[Export Data First]
```

!!! danger "Account Deletion"
    Deleting your account will:

    - Permanently remove all content
    - Delete all chatbots and conversations
    - Cancel your subscription
    - Remove you from all teams
    - **This cannot be undone!**

    Consider exporting your data first.

---

**Previous:** [← Billing & Payments](billing.md) | **Next:** [Security Settings →](security.md)
