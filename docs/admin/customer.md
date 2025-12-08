# Customer Management

Manage company customer accounts with dedicated admin access for enterprise and organizational users.

---

## Overview

The Customer Management system allows you to create and manage company accounts with the following features:
- Company-level customer accounts
- Dedicated customer admin access
- Multi-user company management
- Separate billing and account settings

---

## Accessing Customer Management

Navigate to: **Admin Panel** → **Customer** → **Manage Customer**

---

## Customer List

### Customer Table

The customer management table displays all company customer accounts:

| Column | Description |
|--------|-------------|
| **USER** | Customer account name |
| **ROLE** | Customer Admin (company level) |
| **PHONE** | Contact phone number |
| **EMAIL** | Primary email address |
| **ACTIONS** | Edit or manage customer |

### Current Customers

```
Acme Corporation     | Customer Admin | +1-555-0789  | admin@acmecorp.example
Global Enterprises   | Customer Admin | +1-555-0321  | contact@globalent.example
```

**Total Customers:** 2 company accounts

---

## Creating a New Customer

### Access Creation Form

Navigate to: **Customer** → **Create Customer** or click **"+ New"** button

---

## Customer Creation Form

### Company Information

**Company Name** *(Required)*
```
[Enter company name]
```
- Legal company or organization name
- Appears on invoices and communications
- Used for official documentation

**Company Website**
```
example.com
```
- Company website URL
- Optional but recommended
- Used for verification and branding

**Phone Number**
```
+____________
```
- Company main phone number
- Include country code
- Format: +[country code][number]

**Country**
```
United States ▼
```
- Select from dropdown
- Determines regional settings
- Affects tax calculations and compliance

### Company Address

**Address Line 1** *(Required)*
```
[Enter street address]
```
- Primary company address
- Street and building number

**Address Line 2**
```
[Enter additional address info]
```
- Suite, floor, building name
- Optional details

**City**
```
[Enter city]
```
- Company location city

**State / Province**
```
[Enter state or province]
```
- State, province, or region

**Postal Code**
```
[Enter postal code]
```
- ZIP code or postal code
- Format varies by country

**Description**
```
[Enter description]
```
- Company description
- Business type and industry
- Account notes
- Special requirements or agreements

---

### User Information

This section creates the primary admin user for the customer account.

**First Name** *(Required)*
```
[Enter first name]
```
- Admin user's first name
- Primary account administrator

**Last Name** *(Required)*
```
[Enter last name]
```
- Admin user's last name
- Full name for identification

**Email** *(Required)*
```
[Enter email address]
```
- Must be unique in system
- Login username
- All account communications sent here
- Cannot be changed easily after creation

**Password** *(Required)*
```
[Enter password]
```
- Minimum 8 characters required
- Must be strong and secure
- User can change after first login
- Follow password complexity requirements

!!! note "Password Requirements"
    Password must be at least 8 characters long. For security, include:
    - Uppercase letters (A-Z)
    - Lowercase letters (a-z)
    - Numbers (0-9)
    - Special characters (@, #, $, etc.)

---

### Primary Contact

**Name**
```
[Enter contact name]
```
- Main point of contact
- May be same as admin user
- Day-to-day communications

**Phone Number**
```
+____________
```
- Direct contact number
- For urgent matters
- Include country code

**Email**
```
[Enter contact email]
```
- Contact's email address
- May differ from admin email
- Used for billing and support

**Address (Optional)**
```
[Enter address]
```
- Contact's address if different from company
- Optional field

---

### Saving Customer Account

**To create the customer:**
1. Fill in all required fields (marked with *)
2. Review company and user information
3. Verify email addresses are correct
4. Ensure password meets requirements
5. Click **"Save"** button

**After Creation:**
- Customer account is created
- Admin user account is set up
- Welcome email is sent to admin
- Login credentials are provided
- Customer can access their dashboard

---

## Managing Existing Customers

### Editing Customer Information

**To edit a customer:**
1. Locate customer in the table
2. Click edit icon (✏️) in Actions column
3. Modify desired fields:
   - Company information
   - Contact details
   - Admin user info
   - Account settings
4. Click "Save" to update

**Editable Information:**
- Company details and address
- Contact information
- Admin user details
- Account status
- Billing information

!!! warning "Email Address Changes"
    Changing the admin email requires the user to verify the new address. They will receive a verification link.

### Customer Actions

**Available Actions:**
- **Edit** (✏️) - Modify customer details
- **View Dashboard** - Access customer analytics
- **Manage Users** - Add/remove company users
- **View Billing** - Check subscription and invoices
- **Deactivate** - Suspend customer account
- **Delete** - Remove customer (requires confirmation)

---

## Customer Admin Access

### What Customer Admins Can Do

**Customer Dashboard Access:**
- Manage company users
- Configure company settings
- View company usage statistics
- Access company data only
- Cannot see other customers
- Cannot access platform admin functions

**User Management:**
- Add new users to company
- Remove users from company
- Assign user permissions
- View user activity
- Manage user subscriptions (within company)

**Billing Management:**
- View company invoices
- Update payment methods
- Review usage and costs
- Download receipts
- Manage subscriptions

**Settings:**
- Configure company preferences
- Set branding options
- Manage integrations
- Configure notifications
- Set usage limits

### What Customer Admins Cannot Do

**Restricted Access:**
- ❌ Cannot access platform admin panel
- ❌ Cannot see other companies' data
- ❌ Cannot modify platform settings
- ❌ Cannot create other customer admin accounts
- ❌ Cannot access super admin functions
- ❌ Cannot view platform-wide analytics

---

## Search Functionality

**Search Customers:**
```
🔍 Search Customer name
```

**How to Search:**
1. Enter customer/company name
2. Results filter in real-time
3. Search works on partial names
4. Case-insensitive search
5. Clear to view all customers

---

## Customer Use Cases

### Enterprise Accounts

**Scenario:** Large company with multiple users

**Setup:**
- Create customer account for company
- Assign Customer Admin role
- Customer admin adds company users
- Manage billing at company level
- Centralized usage tracking

**Benefits:**
- Simplified billing
- Centralized management
- Better security control
- Usage oversight
- Team collaboration

### Reseller Customers

**Scenario:** Reseller managing client accounts

**Setup:**
- Reseller creates customer accounts for each client
- Each client gets own customer admin
- Separate billing per customer
- Reseller tracks all clients
- Commission based on customer usage

**Benefits:**
- Clear client separation
- Independent management
- Accurate commission tracking
- Scalable structure

### Agency Partners

**Scenario:** Agency serving multiple clients

**Setup:**
- Agency has main customer account
- Sub-accounts for each client
- Agency manages all accounts
- Clients have read-only access
- Consolidated billing option

**Benefits:**
- Client segregation
- Unified management
- White-label options
- Professional service delivery

---

## Customer Account Management

### Account Status

**Active**
- Full access to platform
- Can create and manage users
- Billing is current
- All features available

**Inactive**
- Login disabled
- Users cannot access platform
- Data is preserved
- Can be reactivated

**Suspended**
- Temporary restriction
- Usually due to payment issues
- Limited access
- Automatically reactivated when resolved

**Deleted**
- Account removed
- Data permanently deleted (after grace period)
- Cannot be recovered
- Email address can be reused

### Billing Management

**Subscription Plans:**
- Company-level subscriptions
- Multiple users under one plan
- Usage-based billing
- Tiered pricing options

**Invoice Handling:**
- Monthly consolidated invoices
- Detailed usage breakdown
- Multiple payment methods
- Auto-billing options

---

## Best Practices

### Creating Customer Accounts

!!! tip "Customer Account Setup"
    **DO:**
    - ✅ Verify company information is accurate
    - ✅ Use company email domain for admin
    - ✅ Set strong password requirements
    - ✅ Document account purpose and details
    - ✅ Send welcome email with instructions

    **DON'T:**
    - ❌ Use personal email addresses
    - ❌ Create duplicates for same company
    - ❌ Skip verification steps
    - ❌ Use weak passwords
    - ❌ Forget to document special agreements

### Ongoing Management

**Regular Activities:**
- Monthly usage review
- Quarterly account check-ins
- Annual contract renewals
- Address issues promptly
- Provide training and support

**Monitoring:**
- Track active users
- Review usage patterns
- Check payment status
- Monitor support tickets
- Assess satisfaction

---

## Multi-User Company Management

### Adding Users to Customer Account

**Customer Admin Process:**
1. Customer Admin logs into dashboard
2. Navigates to User Management
3. Clicks "Add New User"
4. Fills in user details
5. Assigns permissions
6. User receives welcome email

**User Permissions:**
- Full access (same as admin)
- Read-only access
- Limited feature access
- Custom permission sets

### Managing Company Users

**Available Controls:**
- Add/remove users
- Change user permissions
- Reset user passwords
- View user activity
- Deactivate user accounts

---

## Troubleshooting

### Customer Cannot Login

**Issue:** Admin credentials not working

**Solutions:**
1. Verify email address is correct
2. Reset password from login page
3. Check account is active
4. Resend welcome email
5. Create new admin user if needed

### Company Information Incorrect

**Issue:** Wrong company details displayed

**Solutions:**
1. Edit customer account
2. Update company information
3. Save changes
4. Verify updates appear correctly
5. Notify customer of changes

### Multiple Users Issues

**Issue:** Users cannot be added to account

**Solutions:**
1. Check subscription plan limits
2. Verify customer admin permissions
3. Ensure email addresses are unique
4. Review error messages
5. Contact technical support if persists

---

## Customer vs Reseller

### Key Differences

**Customer Account:**
- Company using the platform
- Customer Admin role
- Manages own company users
- Pays for usage directly
- No commission structure

**Reseller Account:**
- Partner selling the platform
- Earns commissions
- Manages multiple customers
- May have custom pricing
- Commission tracking

### When to Use Each

**Use Customer:**
- Direct platform users
- Enterprise companies
- Organizations with multiple users
- Internal team collaboration

**Use Reseller:**
- Partners selling to others
- Agencies with clients
- Distributors
- Affiliate marketers

---

## Reporting and Analytics

### Customer Metrics

**Usage Statistics:**
- Total users
- Active users
- AI operations
- Storage used
- Bandwidth consumed

**Financial Metrics:**
- Monthly recurring revenue
- Usage costs
- Payment history
- Outstanding balance
- Lifetime value

**Engagement Metrics:**
- Login frequency
- Feature adoption
- Support tickets
- User satisfaction
- Retention rate

---

## Additional Resources

**Related Documentation:**
- [Reseller Management](reseller.md) - Compare with reseller accounts
- [User Management](user-management.md) - General user administration
- [Dashboard](dashboard.md) - Monitor customer metrics

---

**Previous:** [← Reseller](reseller.md) | **Next:** [Admin Home →](index.md)
