# User Management

Comprehensive user administration tools for managing platform users, monitoring activities, handling deletion requests, and configuring permissions.

---

## Overview

The User Management section provides complete control over platform users with the following capabilities:

- **Users List** - View and manage all users
- **Users Activities** - Monitor user actions and login history
- **Users Dashboard** - Analyze user metrics and engagement
- **User Deletion Requests** - Handle account deletion requests
- **User Permissions** - Manage admin roles and access levels

---

## Users List

### Accessing User Management

Navigate to: **Admin Panel** → **User Management** → **Users List**

### User List View

The user list displays comprehensive information about all registered users:

| Column | Description |
|--------|-------------|
| **NAME** | User's display name |
| **ROLE** | User, Super Admin, or Customer Admin |
| **WORDS LEFT** | Remaining word generation credits |
| **IMAGES LEFT** | Remaining image generation credits |
| **COUNTRY** | User's country (or Unknown) |
| **STATUS** | Active or Inactive |
| **CREATED AT** | Registration date and time |
| **ACTIONS** | Quick action buttons |

### Sample User Data

```
Emily Anderson     | User          | 0 | 0 | Unknown | Active | 3.11.2025 21:10:50
Robert Martinez    | User          | 0 | 0 | Unknown | Active | 3.11.2025 20:14:22
Lisa Thompson      | User          | 0 | 0 | Unknown | Active | 26.9.2025 06:06:56
James Williams     | User          | 0 | 0 | Unknown | Active | 25.9.2025 16:43:29
Admin User         | Super Admin   | 0 | 0 | Unknown | Active | 17.9.2025 13:05:01
Alice Johnson      | Customer Admin| 0 | 0 | Canada  | Active | 17.9.2025 09:47:32
Thomas Rodriguez   | User          | 0 | 0 | Unknown | Active | 16.9.2025 00:42:06
```

### Search Functionality

**Search Users:**
- Located at top of user list
- Search by user name
- Real-time filtering
- Case-insensitive search

**How to Search:**
1. Click on search field
2. Type user name or partial name
3. Results filter automatically
4. Clear search to view all users

---

## User Actions

### Available Actions

Each user row includes action buttons:

| Icon | Action | Description |
|------|--------|-------------|
| 📋 | View Details | See complete user profile |
| 💲 | Manage Credits | Add/remove words and images credits |
| ✏️ | Edit User | Modify user information |
| ❌ | Delete User | Remove user from platform |

### View User Details

**To view user details:**
1. Click the 📋 icon in Actions column
2. View complete user profile
3. See subscription history
4. Check usage statistics
5. Review activity log

**User Details Include:**
- Personal information
- Contact details
- Subscription plan
- Credit balance
- Registration date
- Last login
- Total usage

### Manage User Credits

**To adjust user credits:**
1. Click the 💲 icon
2. Enter credits to add/remove:
   - Words remaining
   - Images remaining
3. Add note explaining adjustment
4. Save changes

!!! tip "Credit Management"
    Use this feature to:
    - Compensate users for issues
    - Grant promotional credits
    - Adjust for billing errors
    - Reward loyal users

### Edit User Information

**To edit a user:**
1. Click the ✏️ icon
2. Modify user fields:
   - Name
   - Email
   - Password (reset)
   - Role
   - Status
3. Save changes

**Editable Fields:**
- Name
- Email address
- Phone number
- Country
- User role
- Account status
- Custom fields

### Delete User

**To delete a user:**
1. Click the ❌ icon
2. Confirm deletion
3. Choose deletion type:
   - **Soft delete** - Keep data, deactivate account
   - **Hard delete** - Permanently remove all data

!!! warning "Deletion Warning"
    Deleting a user is permanent and cannot be undone. Always verify before deleting.

---

## Export Options

### Export Invoices

**To export invoice data:**
1. Click **"Export Invoices"** button
2. Select date range (optional)
3. Choose format:
   - CSV
   - Excel
   - PDF
4. Download file

**Invoice Export Includes:**
- User name and email
- Invoice date
- Amount
- Payment status
- Subscription plan
- Transaction ID

### Export Users

**To export user list:**
1. Click **"Export Users"** dropdown (⋮)
2. Select export type:
   - All users
   - Active users only
   - Inactive users only
   - Filtered users (current search)
3. Choose format:
   - CSV
   - Excel
   - JSON
4. Download file

**User Export Includes:**
- Name and email
- Role and status
- Credits remaining
- Country
- Registration date
- Last login
- Total usage

---

## Add New User

### Creating a User

**To add a new user:**
1. Click **"+ Add new user"** button
2. Fill in user information:
   - First name
   - Last name
   - Email address
   - Password (minimum 8 characters)
   - Phone number (optional)
   - Country
3. Select user role:
   - User (default)
   - Admin
   - Customer Admin
4. Set initial credits (optional):
   - Words
   - Images
5. Click **"Save"**

**Required Fields:**
- Email address (must be unique)
- Password (minimum 8 characters)
- Name

**Optional Fields:**
- Phone number
- Country
- Initial credits
- Custom fields

!!! note "Email Notifications"
    New users automatically receive a welcome email with login credentials.

---

## User Activities

### Accessing Activity Log

Navigate to: **User Management** → **Users Activities**

### Activity Tracking

The activity log shows detailed user actions:

| Column | Information |
|--------|-------------|
| **EMAIL** | User's email address |
| **USER TYPE** | customer, admin, etc. |
| **IP ADDRESS** | Login IP address |
| **CONNECTION** | Browser and device info |
| **LAST ACTIVITY** | Time since last action |

### Sample Activity Data

```
user@example.com   | customer | 192.168.1.100 | Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15_7) AppleWebKit/537.36... | 2 days ago
user@example.com   | customer | 192.168.1.100 | Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15_7) AppleWebKit/537.36... | 4 days ago
user@example.com   | customer | 192.168.1.100 | Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15_7) AppleWebKit/537.36... | 5 days ago
```

### Activity Insights

**User Activity Tracking:**
- Login timestamps
- IP address monitoring
- Device and browser detection
- User behavior patterns
- Security monitoring

**Use Cases:**
- Detect suspicious logins
- Monitor user engagement
- Track location changes
- Identify inactive users
- Security audits

---

## User Dashboard

### Accessing User Dashboard

Navigate to: **User Management** → **User Dashboard**

### Dashboard Metrics

**Total Registered Users:** 39 (−0%)

**Online Users:** 1

**Visitors Today:** 0

### User Registration Charts

**New Registered Users (Current Month):**
- Graph showing daily registrations
- Currently showing 0 new users
- X-axis: Days 1-31
- Y-axis: Number of users

**Total Registered Users (Current Year):**
- Monthly registration trends
- Peak months identified
- Growth patterns visible
- Historical data available

**Sample Data:**
```
Jan: 0
Feb: 0
Mar: 0
Apr: 1
May: 12
Jun: 3
Jul: 15
Aug: 1
Sep: 5
Oct: 0
Nov: 2
Dec: 0
```

### Dashboard Insights

**Growth Analysis:**
- Peak registration month: July (15 users)
- Second peak: May (12 users)
- Current month: 0 new users
- Annual trend: Decreasing

**Action Items:**
- Investigate low registration periods
- Plan marketing campaigns
- Analyze successful months
- Improve user acquisition

---

## User Deletion Requests

### Accessing Deletion Requests

Navigate to: **User Management** → **User Deletion Requests**

### Deletion Request Table

| Column | Description |
|--------|-------------|
| **USER NAME** | Name of requesting user |
| **USER EMAIL** | User's email address |
| **ACCEPT USER DELETION** | Action button |

### Current Status

```
No users found.
```

### Handling Deletion Requests

**When a request is submitted:**

1. **Review Request:**
   - Check user account status
   - Verify active subscriptions
   - Check for pending payments
   - Review content ownership

2. **Process Request:**
   - Click **"Accept User Deletion"** button
   - Choose deletion type:
     - **Standard** - 30-day grace period
     - **Immediate** - Delete now
   - Confirm action

3. **Data Handling:**
   - Export user data (if requested)
   - Cancel active subscriptions
   - Process final billing
   - Remove personal information
   - Keep anonymous usage stats (optional)

!!! warning "GDPR Compliance"
    User deletion requests must be processed within 30 days to comply with GDPR and similar regulations.

### Best Practices

**Before Accepting Deletion:**
- ✅ Verify user identity
- ✅ Check for active subscriptions
- ✅ Process any refunds
- ✅ Export data if requested
- ✅ Document the deletion

**After Deletion:**
- ✅ Send confirmation email
- ✅ Remove from marketing lists
- ✅ Update analytics
- ✅ Archive necessary records
- ✅ Document compliance

---

## User Permissions

### Accessing Permissions

Navigate to: **User Management** → **User Permissions**

### Admin Permissions System

**Permission Levels:**

1. **Superadmin**
   - Full control over entire system
   - Manage admins and change settings
   - No restrictions

2. **Admin**
   - Control over specific areas
   - Limited to assigned functions
   - Cannot modify system settings

### Admin Privileges

Super admins can control which areas are accessible to regular admins:

**Available Privileges:**

| Privilege | Description |
|-----------|-------------|
| ✓ **Marketplace** | Access to marketplace management |
| ✓ **Themes** | Control theme settings |
| ✓ **User Management** | Manage platform users |
| ✓ **Announcements** | Create and send announcements |
| ✓ **Google AdSense** | Configure advertising |
| ✓ **Support Requests** | Handle support tickets |
| ✓ **Templates** | Manage content templates |
| ✓ **Chat Settings** | Configure chatbot settings |
| ✓ **Frontend** | Modify frontend settings |
| ✓ **Finance** | Access financial data |

### Configuring Admin Access

**To assign admin privileges:**

1. **Select User:**
   - Navigate to Users List
   - Find the admin user
   - Click edit (✏️)

2. **Assign Role:**
   - Change role to "Admin"
   - Save changes

3. **Configure Privileges:**
   - Go to User Permissions
   - Select specific privileges
   - Check boxes for allowed areas
   - Save configuration

4. **Test Access:**
   - Log in as admin user
   - Verify correct access
   - Test restricted areas
   - Confirm permissions work

### Permission Best Practices

!!! tip "Secure Permission Management"
    - **Principle of Least Privilege** - Give minimum necessary access
    - **Regular Audits** - Review permissions quarterly
    - **Role-Based** - Assign permissions by job function
    - **Document Changes** - Keep records of permission changes
    - **Revoke Promptly** - Remove access when no longer needed

---

## User Roles Explained

### User (Standard)

**Default role for all customers:**
- Access to platform features based on subscription
- No admin capabilities
- Cannot view other users
- Limited to personal account

**Permissions:**
- Use all AI tools within plan limits
- Manage personal profile
- View own usage statistics
- Create content and chatbots

### Admin

**Limited administrative access:**
- Manage specific areas as assigned
- Cannot create other admins
- Cannot modify system settings
- Access to assigned privileges only

**Typical Responsibilities:**
- User support
- Content moderation
- Basic reporting
- Assigned functions

### Customer Admin

**Company-level administrator:**
- Manage company users
- Configure company settings
- Access company data only
- No platform-wide access

**Typical Use Cases:**
- Enterprise accounts
- Reseller customers
- Multi-user companies
- Organizational accounts

### Super Admin

**Full platform control:**
- Complete system access
- Manage all admins
- Configure all settings
- Access all data

**Responsibilities:**
- Platform management
- Security oversight
- System configuration
- Final decision authority

---

## Bulk Operations

### Bulk User Management

**Available Bulk Actions:**

1. **Bulk Delete:**
   - Select multiple users (checkboxes)
   - Click bulk delete option
   - Confirm deletion
   - Process all at once

2. **Bulk Credit Assignment:**
   - Select users
   - Choose credit type
   - Enter amount
   - Apply to all selected

3. **Bulk Status Change:**
   - Select users
   - Choose new status (Active/Inactive)
   - Apply change
   - Confirm action

4. **Bulk Export:**
   - Select specific users
   - Export selected only
   - Choose format
   - Download

### Best Practices for Bulk Operations

!!! warning "Use with Caution"
    Bulk operations cannot be easily undone. Always:
    - Double-check selections
    - Verify actions before confirming
    - Create backups first
    - Test on small sample
    - Document bulk changes

---

## Troubleshooting

### Cannot Find User

**Issue:** User doesn't appear in list

**Solutions:**
1. Clear search field
2. Check pagination
3. Verify user exists in database
4. Refresh page
5. Check filters (active/inactive)

### User Deletion Failed

**Issue:** Cannot delete user account

**Possible Causes:**
- Active subscription
- Pending payments
- Linked reseller account
- Database error

**Solutions:**
1. Cancel active subscriptions first
2. Process pending transactions
3. Remove reseller links
4. Contact technical support

### Permission Changes Not Applied

**Issue:** Admin privileges don't update

**Solutions:**
1. Log out and log back in
2. Clear browser cache
3. Wait for permission sync (up to 5 minutes)
4. Verify changes were saved
5. Check for permission conflicts

---

## Security Best Practices

### Protecting User Data

**Data Security:**
- Use HTTPS for all connections
- Encrypt sensitive data
- Regular security audits
- Monitor suspicious activity
- Implement strong password policies

### Access Control

**Admin Access:**
- Use strong, unique passwords
- Enable 2FA for all admins
- Review admin list regularly
- Remove inactive admin accounts
- Log all admin actions

### Privacy Compliance

**Regulations:**
- GDPR compliance
- CCPA compliance
- Data retention policies
- User consent management
- Right to deletion

---

## Additional Resources

**Related Documentation:**
- [Dashboard](dashboard.md) - Platform metrics and analytics
- [Announcements](announcements.md) - Communicate with users
- [Support](support.md) - Handle user support requests

**External Resources:**
- [GDPR Guidelines](https://gdpr.eu/) - Data protection regulations
- [User Privacy Best Practices](#) - Security guidelines

---

**Previous:** [← Dashboard](dashboard.md) | **Next:** [Announcements →](announcements.md)
