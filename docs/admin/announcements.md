# Announcements

Create and manage platform-wide announcements to communicate important information to your users.

---

## Overview

The Announcements system allows you to create two types of announcements:
- **Public Announcements** - Displayed publicly on the platform
- **Dashboard Announcements** - Shown to logged-in users on their dashboard

---

## Accessing Announcements

Navigate to: **Admin Panel** → **Announcements**

---

## Announcement Types

### 1. Public Announcement

**Purpose:** Display announcements visible to all visitors, including non-logged-in users.

**Use Cases:**
- Platform maintenance notifications
- New feature announcements
- Special promotions
- Public service announcements
- General updates

**Creating a Public Announcement:**
1. Navigate to Announcements section
2. Under "1. Public Announcement"
3. Click **"+ New"** button
4. Fill in announcement details

**Table View:**

| Column | Description |
|--------|-------------|
| **TITLE** | Announcement headline |
| **TYPE** | Announcement category |
| **ACTIVE** | On/Off status |
| **ACTION** | Edit or delete |

**Current Status:** No public announcements created yet

---

### 2. Dashboard Announcement

**Purpose:** Display announcements on user dashboards after login.

**Description:** "This announcement will be displayed on the dashboard for all users."

**Use Cases:**
- Welcome messages for new users
- Important account updates
- Feature tutorials
- Tips and best practices
- Promotional offers for logged-in users

### Example Dashboard Announcement

**Title:** Welcome to iQuivity!

**Message:**
"We are excited to have you here. Explore the marketplace to find the best AI models for your needs."

**Actions:**
- **Try it Now** button - Direct link to feature/page
- **Dismiss** button - User can close the announcement

**Announcement Banner:**
```
┌────────────────────────────────────────────────┐
│  📢  Welcome to iQuivity!                     │
│                                                │
│  We are excited to have you here. Explore the │
│  marketplace to find the best AI models for   │
│  your needs.                                   │
│                                                │
│  [Try it Now]  [Dismiss]                      │
└────────────────────────────────────────────────┘
```

---

## Creating an Announcement

### Step 1: Basic Information

**Announcement Status:**
```
Active: [Toggle On/Off]  ⓘ
```

**Title:**
```
Welcome to MagicAI!
```

**Configuration:**
- Toggle Active/Inactive status
- Enter descriptive title
- Title appears as announcement header

---

### Step 2: Visual Customization

**Announcement Icon:**

Default megaphone icon (📢) displayed

**Announcement Background Image (Optional):**
```
[+] Upload Image
```

**Supported Formats:**
- PNG, JPG, GIF
- Recommended size: 1200x400px
- Maximum size: 2MB

**Announcement Background Color:**
```
#ffffff  [Clear]
```

**Color Picker:**
- Enter hex code (#ffffff)
- Use color picker tool
- Clear to use default
- Preview changes live

### Step 3: Content

**Title:**
```
[Enter announcement title]
```

**Message:**
```
[Enter announcement message]
```

**URL (optional):**
```
[Enter URL for "Try it Now" button]
```

**Message Guidelines:**
- Keep concise (2-3 sentences)
- Clear call-to-action
- Highlight key benefit
- Use friendly tone

---

## Announcement Actions

### Save Announcement

**To save your announcement:**
1. Fill in all required fields
2. Click **"Save"** button
3. Announcement is created
4. Toggle active to display

**Actions Available:**
- **Save** - Create/update announcement
- **Reset All Data** - Clear all fields and start over
- **Re-Notify All Users** - Send notification again to all users

### Reset All Data

**Purpose:** Clear all entered information and start fresh.

**How to use:**
1. Click **"Reset All Data"** button
2. All fields cleared
3. Background image removed
4. Color reset to default

!!! warning "Reset Warning"
    This action cannot be undone. All unsaved changes will be lost.

### Re-Notify All Users

**Purpose:** Resend announcement notification to all users, including those who previously dismissed it.

**How to use:**
1. Click **"Re-Notify All Users"** button
2. Confirmation prompt appears
3. Confirm action
4. All users see announcement again

**Use Cases:**
- Critical updates requiring attention
- Announcement was updated with new information
- Ensure all users have seen important message

!!! note "User Experience"
    Users who previously dismissed the announcement will see it again. Use sparingly to avoid notification fatigue.

---

## Managing Announcements

### Edit Announcement

**To edit an existing announcement:**
1. Find announcement in the table
2. Click edit icon (✏️) in ACTION column
3. Modify details as needed
4. Click **"Save"** to update

### Delete Announcement

**To remove an announcement:**
1. Locate announcement in table
2. Click delete icon (🗑️) in ACTION column
3. Confirm deletion
4. Announcement removed from system

!!! warning "Deletion is Permanent"
    Deleted announcements cannot be recovered. Consider deactivating instead of deleting if you might need it later.

### Activate/Deactivate

**To toggle announcement status:**
1. Edit the announcement
2. Toggle the **"Active"** switch
   - **On** - Announcement displays to users
   - **Off** - Announcement hidden but saved
3. Save changes

**Benefits of Deactivating:**
- Keep announcement for future use
- Temporarily hide without deleting
- Preserve all settings and content
- Quick reactivation when needed

---

## Announcement Best Practices

### Content Guidelines

!!! tip "Writing Effective Announcements"
    **DO:**
    - ✅ Keep messages short and clear
    - ✅ Include a clear call-to-action
    - ✅ Use friendly, welcoming tone
    - ✅ Highlight user benefits
    - ✅ Proofread before publishing

    **DON'T:**
    - ❌ Write long paragraphs
    - ❌ Use technical jargon
    - ❌ Overuse exclamation marks!!!
    - ❌ Include too many links
    - ❌ Forget to test the URL

### Visual Design

**Background Images:**
- Use high-quality images
- Ensure text is readable
- Match brand colors
- Optimize file size
- Test on mobile devices

**Background Colors:**
- Use brand colors
- Ensure sufficient contrast
- Test readability
- Consider accessibility
- Preview before publishing

### Timing and Frequency

**When to Send Announcements:**
- Major platform updates
- New feature launches
- Important security updates
- Scheduled maintenance
- Special promotions

**Frequency Guidelines:**
- **Maximum:** 1 per week for general updates
- **Critical updates:** As needed
- **Promotions:** 2-3 per month maximum
- **Seasonal:** Around holidays or events

!!! warning "Avoid Announcement Fatigue"
    Too many announcements can lead to users ignoring them or becoming annoyed. Use announcements sparingly for truly important messages.

---

## Examples and Templates

### Welcome Announcement

**Title:** Welcome to iQuivity!

**Message:**
"We're excited to have you here. Explore our AI tools to create amazing content, images, and videos in seconds."

**URL:** `/dashboard`

**Background Color:** `#5B21B6` (Purple)

**Button Text:** "Get Started"

---

### New Feature Announcement

**Title:** Introducing AI Video Pro!

**Message:**
"Create professional videos from URLs with our new AI Video Pro feature. Try it now and see the magic happen!"

**URL:** `/ai-videos/video-pro`

**Background Color:** `#2563EB` (Blue)

**Button Text:** "Try AI Video Pro"

---

### Maintenance Notice

**Title:** Scheduled Maintenance

**Message:**
"We'll be performing system upgrades on Saturday, Dec 10 at 2 AM EST. Platform will be unavailable for approximately 2 hours. Thank you for your patience!"

**URL:** `/status`

**Background Color:** `#F59E0B` (Orange)

**Button Text:** "View Status"

---

### Promotional Announcement

**Title:** Limited Time: 50% Off Pro Plan!

**Message:**
"Upgrade to Pro and get 50% off your first month. Offer ends Dec 31. Don't miss out on unlimited AI generation!"

**URL:** `/pricing`

**Background Color:** `#DC2626` (Red)

**Button Text:** "Upgrade Now"

---

## Announcement Analytics

### Tracking Performance

**Metrics to Monitor:**
- **Impressions** - How many users saw the announcement
- **Click-through Rate** - Users who clicked the CTA button
- **Dismissal Rate** - Users who dismissed without action
- **Time to Dismiss** - How quickly users dismissed

### Analyzing Effectiveness

**Good Announcement Indicators:**
- High click-through rate (>10%)
- Low dismissal rate (<30%)
- Longer viewing time
- Positive user feedback

**Poor Announcement Indicators:**
- Immediate dismissals
- No clicks on CTA
- User complaints
- High dismissal rate (>70%)

---

## Troubleshooting

### Announcement Not Displaying

**Issue:** Users don't see the announcement

**Solutions:**
1. Check Active status is ON
2. Verify announcement type (Public vs Dashboard)
3. Clear user browser cache
4. Check for JavaScript errors
5. Test in different browser

### Broken CTA Button

**Issue:** "Try it Now" button doesn't work

**Solutions:**
1. Verify URL is correct
2. Check URL starts with `/` or `https://`
3. Test URL in browser
4. Ensure no typos in link
5. Check URL permissions

### Background Image Not Loading

**Issue:** Background image doesn't appear

**Solutions:**
1. Check image file size (<2MB)
2. Verify image format (PNG, JPG, GIF)
3. Re-upload image
4. Clear cache
5. Try different image

---

## Additional Resources

**Related Documentation:**
- [User Management](user-management.md) - Manage announcement recipients
- [Dashboard](dashboard.md) - Monitor announcement engagement

---

**Previous:** [← User Management](user-management.md) | **Next:** [Support →](support.md)
