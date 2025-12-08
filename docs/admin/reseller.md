# Reseller Management

Manage reseller partnerships, track commissions, and oversee reseller accounts.

---

## Overview

The Reseller Management system allows you to:
- Create and manage reseller accounts
- Track commissions and payouts
- Monitor reseller performance
- Configure reseller settings

---

## Accessing Reseller Management

Navigate to: **Admin Panel** → **Reseller** → **Manage Reseller**

---

## Reseller List

### Reseller Table

The reseller management table displays all active reseller partnerships:

| Column | Description |
|--------|-------------|
| **RESELLER NAME** | Company or individual name |
| **PHONE NUMBER** | Contact phone |
| **ADDRESS** | Business address |
| **CREATED BY** | Admin who created account |
| **ACTIONS** | Edit or manage reseller |

### Current Resellers

```
TechCo Solutions | +1-555-0123        | 123 Business Park Drive    | Admin User
Digital Dynamics | +1-555-0456        | 456 Commerce Street        | Admin User
```

**Total Resellers:** 2 active partnerships

---

## Creating a New Reseller

### Access Creation Form

Navigate to: **Reseller** → **Create Reseller** or click **"+ New"** button

---

## Reseller Creation Form

### Company Information

**Company Name** *(Required)*
```
[Enter company name]
```
- Legal business name
- Will appear on invoices
- Used for official communications

**Company Website**
```
example.com
```
- Business website URL
- Optional but recommended
- Used for verification

**Phone Number**
```
+____________
```
- Include country code
- Format: +[country code][number]
- Primary contact number

**Country**
```
[Select Country ▼]
```
- Choose from dropdown
- Determines tax and legal requirements
- Affects commission structure

### Address Information

**Address Line 1** *(Required)*
```
[Enter street address]
```
- Primary business address
- Street and building number

**Address Line 2**
```
[Enter additional address info]
```
- Suite, apartment, floor number
- Optional additional details

**City**
```
[Enter city]
```
- Business location city

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
- Business description
- Partnership details
- Any additional notes

---

### Commission Settings

**Commission** *(Required)*
```
[Enter commission amount]
```
- Percentage or flat rate
- Per sale or recurring
- Clearly define structure

**Type**
```
[Select Type ▼]
```

**Commission Types:**
- **Percentage** - % of each sale
- **Flat Rate** - Fixed amount per sale
- **Tiered** - Varies by volume
- **Recurring** - Ongoing subscription commission

---

### Admin Information

**First Name** *(Required)*
```
[Enter first name]
```
- Admin user first name
- Access to reseller dashboard

**Last Name** *(Required)*
```
[Enter last name]
```
- Admin user last name
- Full name for account

**Email** *(Required)*
```
[Enter email address]
```
- Must be unique
- Login credentials sent here
- Used for all communications

**Password** *(Required)*
```
[Enter password]
```
- Minimum 8 characters
- Must be strong and secure
- Admin account password

!!! note "Password Requirements"
    Password must be at least 8 characters long. Include uppercase, lowercase, numbers, and special characters for best security.

---

### Billing Information

**Billing Address Line 1**
```
[Enter billing address]
```
- Where invoices are sent
- May differ from business address

**Billing Address Line 2**
```
[Enter additional billing info]
```
- Optional additional details

**City**
```
[Enter city]
```
- Billing address city

**State**
```
[Enter billing state]
```
- Billing state or province

**Zip Code**
```
[Enter zip code]
```
- Billing postal code

---

### Primary Contact

**Name**
```
[Enter contact name]
```
- Main point of contact
- Day-to-day communications

**Phone Number**
```
+____________
```
- Direct contact number
- For urgent matters

**Email**
```
[Enter contact email]
```
- Contact's email address
- May differ from admin email

**Address (Optional)**
```
[Enter address]
```
- Contact's address if different

---

### Saving Reseller

**To create the reseller:**
1. Fill in all required fields (marked with *)
2. Review all information for accuracy
3. Click **"Save"** button
4. Reseller account is created
5. Admin login credentials are emailed

---

## Managing Existing Resellers

### Editing Reseller Information

**To edit a reseller:**
1. Locate reseller in the table
2. Click edit icon (✏️) in Actions column
3. Modify desired fields
4. Click "Save" to update

**Editable Information:**
- Company details
- Contact information
- Commission structure
- Admin credentials
- Billing information

### Reseller Actions

**Available Actions:**
- **Edit** (✏️) - Modify reseller details
- **View Dashboard** - Access reseller analytics
- **View Commissions** - Check payment history
- **Deactivate** - Suspend reseller account
- **Delete** - Remove reseller (with confirmation)

---

## Commission Tracking

### Accessing Commissions

Navigate to: **Reseller** → **Commissions**

### Commission Table

| Column | Description |
|--------|-------------|
| **COMMISSION** | Amount owed |
| **EARNED BY** | Reseller name |
| **STATUS** | Pending, Paid, Processing |
| **CREATED AT** | When commission was earned |

### Current Status

```
No commission records found.
```

**When commissions are earned:**
- Automatically tracked
- Calculated based on sales
- Updated in real-time
- Ready for payout processing

---

## Commission Structure Examples

### Percentage Commission

**Example: 10% commission**
- Sale: $100
- Commission: $10
- Reseller receives: $10 per sale

### Flat Rate Commission

**Example: $5 per sale**
- Regardless of sale amount
- Consistent earnings
- Predictable payouts

### Tiered Commission

**Example: Volume-based**
- 1-10 sales: 5%
- 11-50 sales: 10%
- 51+ sales: 15%

### Recurring Commission

**Example: Subscription-based**
- Monthly subscription: $50
- Commission: 20% ($10/month)
- Ongoing as long as customer subscribed

---

## Reseller Dashboard Access

### What Resellers Can See

**Reseller Dashboard Includes:**
- Commission earnings
- Sales statistics
- Customer list
- Payment history
- Referral links
- Marketing materials
- Performance analytics

**Reseller Capabilities:**
- View own sales and commissions
- Track customer subscriptions
- Access referral tools
- Generate reports
- Update profile information
- Cannot access other resellers' data
- Cannot modify platform settings

---

## Processing Commissions

### Payment Workflow

**1. Commission Earned:**
- Customer makes purchase through reseller link
- Commission automatically calculated
- Added to pending commissions

**2. Review Period:**
- Minimum holding period (e.g., 30 days)
- Verify sale is not refunded
- Confirm customer is active

**3. Process Payment:**
- Navigate to Commissions table
- Select commissions to pay
- Process payment via bank transfer
- Mark as "Paid"
- Send confirmation to reseller

**4. Record Keeping:**
- Transaction logged
- Email receipt sent
- Updated in financial reports
- Available for tax reporting

### Payment Methods

**Supported Methods:**
- Bank transfer (ACH, wire)
- PayPal
- Check (mail)
- Direct deposit
- Payment platform (Stripe, etc.)

---

## Reseller Performance Metrics

### Key Metrics to Track

**Sales Volume:**
- Total sales generated
- Number of customers referred
- Average order value
- Conversion rate

**Commission Earnings:**
- Total earned
- Total paid
- Outstanding balance
- Historical trends

**Customer Retention:**
- Active subscriptions
- Churn rate
- Customer lifetime value
- Repeat purchases

**Engagement:**
- Logins to reseller dashboard
- Marketing material downloads
- Support requests
- Communication frequency

---

## Reseller Best Practices

### Partner Selection

!!! tip "Choosing Quality Resellers"
    - **Verify Business** - Check legitimacy and reputation
    - **Assess Audience** - Ensure alignment with platform
    - **Review Experience** - Consider previous partnerships
    - **Check References** - Contact other platforms they work with
    - **Set Clear Expectations** - Define goals and requirements

### Onboarding Process

**New Reseller Onboarding:**

1. **Welcome Email:**
   - Login credentials
   - Getting started guide
   - Commission structure details
   - Key contacts

2. **Training Session:**
   - Platform overview
   - Reseller dashboard walkthrough
   - Marketing materials review
   - Best practices sharing

3. **Provide Resources:**
   - Referral links
   - Marketing collateral
   - Product documentation
   - FAQ and support info

4. **Set Goals:**
   - Monthly sales targets
   - Commission milestones
   - Growth objectives
   - Performance metrics

### Ongoing Management

**Regular Activities:**
- Monthly performance reviews
- Quarterly business reviews
- Provide marketing updates
- Share new features and promotions
- Process commissions on schedule
- Address concerns promptly

---

## Marketing Support for Resellers

### Provided Materials

**Standard Package:**
- Referral links (tracked)
- Banner ads (various sizes)
- Email templates
- Social media posts
- Product brochures
- Video demonstrations
- Case studies
- Testimonials

**Custom Materials:**
- Co-branded collateral
- Custom landing pages
- Personalized demos
- White-label options
- Dedicated support

---

## Troubleshooting

### Reseller Cannot Login

**Issue:** Admin account credentials not working

**Solutions:**
1. Reset password from login page
2. Verify email address is correct
3. Check account is active
4. Resend welcome email
5. Create new admin user if needed

### Commission Not Tracking

**Issue:** Sales not appearing in commission table

**Solutions:**
1. Verify referral link was used
2. Check tracking cookie settings
3. Confirm sale meets commission criteria
4. Review commission rules
5. Manually add commission if verified

### Payment Issues

**Issue:** Cannot process commission payment

**Solutions:**
1. Verify bank information is current
2. Check minimum payout threshold
3. Confirm no pending holds
4. Review payment method settings
5. Contact finance team if persists

---

## Reseller Agreement

### Key Contract Terms

**Standard Agreement Includes:**
- Commission structure
- Payment terms
- Marketing guidelines
- Territory restrictions (if any)
- Exclusivity clauses (if any)
- Termination conditions
- Confidentiality requirements
- Liability limitations

**Important Clauses:**
- Commission eligibility
- Payment schedule
- Refund policy impact
- Intellectual property rights
- Dispute resolution
- Agreement duration

---

## Search Functionality

**Search Resellers:**
```
🔍 Search Reseller name
```

**How to Search:**
1. Enter reseller company name
2. Results filter in real-time
3. Search partial names
4. Case-insensitive
5. Clear to show all

---

## Additional Resources

**Related Documentation:**
- [Commissions](support.md#withdrawal-requests) - Process payments
- [User Management](user-management.md) - Manage reseller admin accounts
- [Dashboard](dashboard.md) - Monitor reseller performance

---

**Previous:** [← Support](support.md) | **Next:** [Customer →](customer.md)
