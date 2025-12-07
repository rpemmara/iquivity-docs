# Security Settings

Protect your account with advanced security features including Two-Factor Authentication, password management, and session monitoring.

## Two-Factor Authentication (2FA)

Add an extra layer of security to your account with 2FA.

### What is Two-Factor Authentication?

2FA requires two forms of verification when logging in:
1. **Something you know** - Your password
2. **Something you have** - Your phone or authentication app

This prevents unauthorized access even if someone obtains your password.

### Enabling 2FA

#### Method 1: Authenticator App (Recommended)

**Step 1: Navigate to Settings**
- Go to **Settings** → **Security** → **Two-Factor Authentication**

**Step 2: Choose Method**
- Select **"Authenticator App"**

**Step 3: Install Authenticator App**

Compatible apps:
- Google Authenticator (iOS, Android)
- Microsoft Authenticator (iOS, Android)
- Authy (iOS, Android, Desktop)
- 1Password
- LastPass Authenticator

**Step 4: Scan QR Code**

```
┌────────────────────────────┐
│  Scan this QR code with    │
│  your authenticator app:   │
│                            │
│  ████████████████████      │
│  ██      ██████    ██      │
│  ██  ██  ██    ██  ██      │
│  ██  ██  ██  ████  ██      │
│  ██      ████  ██████      │
│  ████████████████████      │
│                            │
│  Or enter this key manually:│
│  ABCD EFGH IJKL MNOP       │
│                            │
└────────────────────────────┘
```

**Step 5: Enter Verification Code**

```
Enter the 6-digit code from your app:

┌───┬───┬───┬───┬───┬───┐
│ 1 │ 2 │ 3 │ 4 │ 5 │ 6 │
└───┴───┴───┴───┴───┴───┘

[Verify]
```

**Step 6: Save Backup Codes**

```
⚠️  IMPORTANT: Save these backup codes!

Use these codes if you lose access to your
authenticator app. Each code can only be used once.

Backup Codes:
1. ABCD-1234-EFGH-5678
2. IJKL-9012-MNOP-3456
3. QRST-7890-UVWX-1234
4. YZAB-4567-CDEF-8901
5. GHIJ-2345-KLMN-6789
6. OPQR-0123-STUV-4567
7. WXYZ-7890-ABCD-1234
8. EFGH-3456-IJKL-7890

[Download as Text]  [Print]  [Copy All]

☑ I have saved these codes in a secure location
```

!!! warning "Save Backup Codes"
    Store backup codes in a secure location like a password manager or safe. Without them, you could lose access to your account if you lose your phone!

#### Method 2: SMS Verification

**Step 1: Choose SMS Method**
- Select **"SMS Verification"**

**Step 2: Enter Phone Number**

```
Phone Number for SMS:
┌──────────────────────────────┐
│ Country: [United States ▼]   │
│ Phone: [+1 (555) 123-4567]  │
└──────────────────────────────┘

[Send Verification Code]
```

**Step 3: Verify Phone**
- Receive SMS with 6-digit code
- Enter code to verify
- 2FA is now enabled

!!! note "SMS vs Authenticator App"
    Authenticator apps are more secure than SMS because:

    - SMS can be intercepted
    - SIM swapping attacks are possible
    - Works without cell signal
    - Faster and more reliable

    We recommend using an authenticator app when possible.

### Using 2FA to Login

**Login Process with 2FA:**

1. Enter email and password as usual
2. Prompted for verification code
3. Open authenticator app
4. Enter the 6-digit code
5. Successfully logged in

```
┌────────────────────────────────┐
│ Two-Factor Authentication      │
├────────────────────────────────┤
│                                │
│ Enter your 6-digit code:       │
│                                │
│ ┌───┬───┬───┬───┬───┬───┐    │
│ │   │   │   │   │   │   │    │
│ └───┴───┴───┴───┴───┴───┘    │
│                                │
│ ☐ Trust this device for 30 days│
│                                │
│ [Verify]                       │
│                                │
│ Lost your device?              │
│ [Use backup code]              │
│                                │
└────────────────────────────────┘
```

**Trust Device Option:**
- Check "Trust this device" to skip 2FA for 30 days
- Only use on personal, secure devices
- Not recommended for shared/public computers

### Backup Codes

**What are Backup Codes?**
- One-time use codes
- Used when you don't have access to 2FA device
- 8 codes provided initially
- Generate new codes at any time

**Using a Backup Code:**
1. At 2FA prompt, click **"Use backup code"**
2. Enter one of your saved backup codes
3. Code is consumed (one-time use)
4. Successfully logged in

**Regenerating Backup Codes:**

```
Backup Codes
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Codes remaining: 6/8

⚠️  Warning: Generating new codes will
    invalidate all existing codes.

[Regenerate Codes]
[View Current Codes]
```

### Disabling 2FA

**To Disable 2FA:**

1. Go to **Settings** → **Security** → **Two-Factor Authentication**
2. Click **"Disable 2FA"**
3. Enter current password
4. Enter 2FA code or backup code
5. Confirm disabling

!!! danger "Security Risk"
    Disabling 2FA makes your account less secure. Only disable if absolutely necessary.

## Password Management

### Changing Your Password

**Update Password:**

```
┌─────────────────────────────────────┐
│ Change Password                     │
├─────────────────────────────────────┤
│                                     │
│ Current Password                    │
│ [************************]          │
│                                     │
│ New Password                        │
│ [************************]          │
│                                     │
│ Password Strength: Strong ✓         │
│ ████████████████████                │
│                                     │
│ Confirm New Password                │
│ [************************]          │
│                                     │
│ Requirements:                       │
│ ✓ At least 8 characters             │
│ ✓ At least one uppercase letter     │
│ ✓ At least one lowercase letter     │
│ ✓ At least one number               │
│ ✓ At least one special character    │
│ ✓ Not a commonly used password      │
│                                     │
│ [Change Password]  [Cancel]         │
└─────────────────────────────────────┘
```

### Password Requirements

**Strong Password Guidelines:**

✅ **Do:**
- Use 12+ characters (longer is better)
- Mix uppercase and lowercase
- Include numbers and symbols
- Use a unique password
- Use a password manager

❌ **Don't:**
- Use personal information (name, birthday)
- Use common words or patterns (password123)
- Reuse passwords from other sites
- Share your password
- Write it down in plain text

**Password Strength Meter:**
```
Weak:     ████░░░░░░░░░░░░░░░░
Fair:     ████████░░░░░░░░░░░░
Good:     ████████████░░░░░░░░
Strong:   ████████████████░░░░
Excellent:████████████████████
```

### Password Reset

**If You Forget Your Password:**

1. Click **"Forgot Password?"** on login page
2. Enter your registered email
3. Check email for reset link
4. Click link (valid for 1 hour)
5. Create new password
6. Log in with new password

!!! note "Password Reset Email"
    If you don't receive the email:

    - Check spam/junk folder
    - Verify you entered the correct email
    - Wait 5 minutes and try again
    - Contact support if still not received

## Active Sessions

Monitor and manage all devices logged into your account.

### Session Management

**View Active Sessions:**

```
┌─────────────────────────────────────────────────────┐
│ Active Sessions                                     │
├─────────────────────────────────────────────────────┤
│                                                     │
│ 🖥️  Current Session                                 │
│ Chrome on macOS - New York, USA                     │
│ Last active: Just now                               │
│ IP: 192.168.1.100                                   │
│                                                     │
│ 📱 iPhone - Safari                                  │
│ iOS - New York, USA                                 │
│ Last active: 2 hours ago                            │
│ IP: 192.168.1.105                                   │
│ [End Session]                                       │
│                                                     │
│ 💻 Chrome on Windows                                │
│ Windows 11 - Los Angeles, USA                       │
│ Last active: 1 day ago                              │
│ IP: 198.51.100.42                                   │
│ [End Session]                                       │
│                                                     │
│ [End All Other Sessions]                            │
└─────────────────────────────────────────────────────┘
```

**Session Information:**
- Device type and browser
- Operating system
- Location (approximate)
- IP address
- Last active time

**Managing Sessions:**
- End individual sessions remotely
- End all sessions except current
- Review for unauthorized access
- Requires password and 2FA to end sessions

### Login History

**View Login Activity:**

```
Login History (Last 30 Days)

✓ Dec 2, 2024 10:30 AM - Chrome, macOS, New York
✓ Dec 2, 2024 8:15 AM - Safari, iOS, New York
✓ Dec 1, 2024 3:45 PM - Chrome, macOS, New York
✓ Dec 1, 2024 9:00 AM - Chrome, macOS, New York
✗ Nov 30, 2024 11:22 PM - Chrome, Windows, Unknown
  ⚠️  Failed login attempt
✓ Nov 30, 2024 2:30 PM - Chrome, macOS, New York

[View Full History]  [Export CSV]
```

**Suspicious Activity Alerts:**
- Failed login attempts
- Login from new device
- Login from unusual location
- Multiple failed attempts

## Security Alerts

### Email Notifications

Receive alerts for important security events:

```
Security Notifications:
☑ New device login
☑ Password changed
☑ Email address changed
☑ 2FA enabled/disabled
☑ Failed login attempts (3+)
☑ Account settings changed
☑ API key created/deleted
☑ Unusual activity detected
```

### Security Dashboard

**Account Security Overview:**

```
╔════════════════════════════════════╗
║ Security Score: 92/100 ⭐⭐⭐⭐⭐   ║
╠════════════════════════════════════╣
║ ✅ Strong password                 ║
║ ✅ 2FA enabled (Authenticator)     ║
║ ✅ Email verified                  ║
║ ✅ Phone verified                  ║
║ ⚠️  1 API key never used (review)  ║
║ ✅ No suspicious activity          ║
║ ✅ Recent login review (2 days)    ║
╚════════════════════════════════════╝

Recommendations:
• Review unused API key
• Update recovery phone number
```

## API Security

### API Keys

**Manage API Keys:**

```
┌─────────────────────────────────────────────────────┐
│ API Keys                                            │
├─────────────────────────────────────────────────────┤
│                                                     │
│ Production API Key                                  │
│ sk_live_••••••••••••••••1234                       │
│ Created: Nov 15, 2024                               │
│ Last used: 2 hours ago                              │
│ [Regenerate]  [Delete]                              │
│                                                     │
│ Testing API Key                                     │
│ sk_test_••••••••••••••••5678                       │
│ Created: Nov 1, 2024                                │
│ Last used: Never                                    │
│ [Regenerate]  [Delete]                              │
│                                                     │
│ [Create New API Key]                                │
└─────────────────────────────────────────────────────┘
```

**API Key Best Practices:**
- Never share API keys
- Use different keys for different environments
- Regenerate keys regularly
- Delete unused keys
- Monitor API usage for anomalies
- Store keys securely (use environment variables)

### Regenerating API Keys

**When to Regenerate:**
- Key may have been compromised
- Regular security rotation (every 90 days)
- Team member with access leaves
- Suspicious API activity detected

**How to Regenerate:**
1. Click **"Regenerate"** on API key
2. Confirm regeneration
3. Old key immediately invalidated
4. Copy new key (shown once)
5. Update applications with new key

!!! warning "Key Regeneration"
    Regenerating a key immediately invalidates the old key. All applications using the old key will stop working until updated!

## Connected Devices

**Manage Authorized Devices:**

```
Authorized Devices

📱 iPhone 13 Pro
   Added: Oct 1, 2024
   Last active: Today
   [Remove Device]

💻 MacBook Pro
   Added: Sep 15, 2024
   Last active: Today
   [Remove Device]

🖥️  Windows Desktop
   Added: Aug 10, 2024
   Last active: 3 days ago
   [Remove Device]

[Remove All Devices]
```

## Data Protection

### Encryption

**Data Security Measures:**

✅ **In Transit:**
- TLS 1.3 encryption
- HTTPS only
- Certificate pinning

✅ **At Rest:**
- AES-256 encryption
- Encrypted backups
- Secure data centers

✅ **End-to-End:**
- Encrypted file storage
- Encrypted API communications
- Zero-knowledge options (Enterprise)

### Privacy Controls

```
Privacy Settings:
☑ Encrypt uploaded files
☑ Enable enhanced privacy mode
☑ Require encryption for exports
☐ Enable zero-knowledge mode (Enterprise)
```

## Security Best Practices

### Recommended Security Setup

✅ **Essential:**
- [x] Use strong, unique password
- [x] Enable 2FA with authenticator app
- [x] Verify email and phone
- [x] Review active sessions regularly

✅ **Recommended:**
- [x] Set up security alerts
- [x] Review login history monthly
- [x] Use password manager
- [x] Keep backup codes secure

✅ **Advanced:**
- [x] Regenerate API keys quarterly
- [x] Review connected apps monthly
- [x] Enable enhanced privacy features
- [x] Use separate accounts for testing

### Security Checklist

**Monthly Review:**
- [ ] Check active sessions
- [ ] Review login history
- [ ] Update recovery information
- [ ] Check for security alerts
- [ ] Review API key usage

**Quarterly Review:**
- [ ] Change password
- [ ] Regenerate API keys
- [ ] Review connected devices
- [ ] Update security questions
- [ ] Audit team member access

---

**Previous:** [← Profile Settings](profile.md) | **Next:** [Subscription & Billing →](billing.md)
