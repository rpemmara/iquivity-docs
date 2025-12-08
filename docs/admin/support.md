# Support Requests

Manage user support tickets, affiliate requests, and withdrawal requests from the admin panel.

---

## Overview

The Support section handles three types of requests:
- **Support Requests** - User help tickets and technical issues
- **Affiliate Requests** - Partnership and affiliate program applications
- **Withdrawal Requests** - Payout and refund requests

---

## Accessing Support

Navigate to: **Admin Panel** → **Support Requests**

---

## Support Requests

### Support Ticket Table

The support requests table displays all user-submitted tickets:

| Column | Description |
|--------|-------------|
| **TICKET ID** | Unique ticket identifier |
| **STATUS** | Open, In Progress, Resolved, Closed |
| **CATEGORY** | Type of support request |
| **SUBJECT** | Brief description of issue |
| **PRIORITY** | Low, Medium, High, Urgent |
| **CREATED AT** | When ticket was submitted |
| **LAST UPDATED** | Most recent activity |
| **ACTIONS** | View, respond, close |

### Current Status

```
No support requests found
```

**When tickets are submitted, they will appear here with:**
- Unique ticket ID for tracking
- Current status indicator
- Category classification
- User information
- Priority level
- Creation and update timestamps

---

## Handling Support Requests

### Viewing Tickets

**To view a support ticket:**
1. Locate ticket in table
2. Click on ticket ID or view icon
3. See complete ticket details:
   - User information
   - Full description
   - Attached files/screenshots
   - Conversation history
   - Related tickets

### Responding to Tickets

**To respond:**
1. Open the ticket
2. Click "Reply" or "Add Response"
3. Type your response
4. Attach files if needed
5. Set status (In Progress, Resolved, etc.)
6. Click "Send"

**Response Best Practices:**
- Acknowledge ticket within 24 hours
- Be clear and concise
- Provide step-by-step solutions
- Ask clarifying questions if needed
- Set realistic expectations
- Follow up on resolution

### Updating Ticket Status

**Status Options:**

**Open** - New, unassigned ticket
- Just submitted
- Not yet reviewed
- Awaiting assignment

**In Progress** - Being worked on
- Assigned to support staff
- Investigation underway
- Awaiting information

**Resolved** - Solution provided
- Issue addressed
- Awaiting user confirmation
- Can be reopened if needed

**Closed** - Completed
- User confirmed resolution
- No further action needed
- Archived for reference

### Prioritizing Tickets

**Priority Levels:**

**Low** - General questions, non-urgent
- Response time: 48-72 hours
- Can be batched
- Scheduled support

**Medium** - Standard issues (Default)
- Response time: 24-48 hours
- Regular workflow
- Most common

**High** - Affecting user's work
- Response time: 4-8 hours
- Priority handling
- Escalate if needed

**Urgent** - Critical issues, outages
- Response time: 1-2 hours
- Immediate attention
- All hands on deck

---

## Affiliate Requests

### Affiliate Program Overview

The Affiliate Requests section manages applications to the affiliate/referral program.

### Affiliate Request Table

| Column | Description |
|--------|-------------|
| **#** | Request number |
| **NAME** | Applicant name |
| **EMAIL** | Contact email |
| **WEBSITE** | Affiliate website/platform |
| **AUDIENCE** | Target audience description |
| **STATUS** | Pending, Approved, Rejected |
| **DATE** | Application date |
| **ACTIONS** | Approve, reject, view details |

### Current Status

```
There is no withdrawal request
```

### Reviewing Affiliate Applications

**To review an application:**
1. Click on application to view details
2. Review applicant information:
   - Name and contact details
   - Website/platform information
   - Audience size and demographics
   - Promotional methods
   - Previous affiliate experience
3. Verify website is legitimate
4. Check audience alignment
5. Approve or reject application

### Approving Affiliates

**To approve:**
1. Review application thoroughly
2. Click "Approve" button
3. Set commission rate (if custom)
4. Provide affiliate link and materials
5. Send welcome email with:
   - Affiliate dashboard access
   - Unique referral link
   - Commission structure
   - Promotional materials
   - Program guidelines

### Rejecting Applications

**To reject:**
1. Click "Reject" button
2. Provide reason for rejection (optional)
3. Send notification to applicant
4. Document decision

**Common Rejection Reasons:**
- Inappropriate website content
- Misaligned audience
- Incomplete application
- Previous policy violations
- Duplicate application

---

## Withdrawal Requests

### Withdrawal Overview

Manage payout and refund requests from users, affiliates, and resellers.

### Withdrawal Request Table

| Column | Description |
|--------|-------------|
| **#** | Request ID |
| **AMOUNT** | Requested payout amount |
| **BANK INFORMATION** | Payment details |
| **STATUS** | Pending, Approved, Processed, Rejected |
| **DATE** | Request submission date |
| **ACTION** | Process, view, decline |

### Current Status

```
There is no withdrawal request
```

### Processing Withdrawals

**To process a withdrawal:**

1. **Verify Request:**
   - Check user balance
   - Verify minimum payout threshold
   - Confirm bank details
   - Check for pending holds

2. **Validate Amount:**
   - Ensure sufficient balance
   - Deduct processing fees
   - Check for discrepancies
   - Verify calculation

3. **Process Payment:**
   - Initiate bank transfer
   - Update status to "Processing"
   - Record transaction
   - Deduct from user balance

4. **Confirm Completion:**
   - Mark as "Processed"
   - Send confirmation email
   - Provide transaction reference
   - Update financial records

### Successful Withdrawal Table

**Completed withdrawals display in separate table:**

| Column | Description |
|--------|-------------|
| **#** | Transaction ID |
| **AMOUNT** | Paid amount |
| **BANK INFORMATION** | Payment method used |
| **STATUS** | Completed |
| **DATE** | Processing date |
| **ACTION** | View receipt, details |

### Current Status

```
There is no successful withdrawal request
```

### Withdrawal Best Practices

!!! tip "Processing Withdrawals"
    - **Verify All Details** - Double-check amounts and bank info
    - **Process Timely** - Within 3-5 business days
    - **Communicate** - Keep users informed of status
    - **Document Everything** - Keep records of all transactions
    - **Watch for Fraud** - Flag suspicious patterns

---

## Support Metrics and Reporting

### Key Support Metrics

**Response Time:**
- Average time to first response
- Average time to resolution
- Ticket backlog

**Ticket Volume:**
- Total tickets per day/week/month
- Tickets by category
- Tickets by priority

**Resolution Rate:**
- Percentage of resolved tickets
- Reopen rate
- Customer satisfaction score

**Common Issues:**
- Most frequent ticket categories
- Trending problems
- Feature requests

### Generating Reports

**Available Reports:**
- Support ticket summary (daily, weekly, monthly)
- Response time analysis
- Agent performance
- Category breakdown
- Resolution trends

---

## Coupons Management

### Creating Discount Coupons

Navigate to: **Manage Coupons**

**To create a coupon:**
1. Click **"+ Add New Coupon"** button
2. Enter coupon details:
   - **Name** - Internal reference
   - **Code** - User-facing coupon code
   - **Discount (%)** - Percentage off
   - **Limit** - Maximum uses
   - **Created By** - Admin name
3. Click "Save"

### Coupon Table

| Column | Description |
|--------|-------------|
| **NAME** | Coupon name/description |
| **CODE** | Redemption code |
| **DISCOUNT (%)** | Discount amount |
| **LIMIT** | Maximum redemptions |
| **USED** | Times redeemed |
| **CREATED BY** | Admin who created |
| **ACTION** | Edit, delete, deactivate |

### Current Status

```
There is no coupons yet
```

### Coupon Best Practices

**Creating Effective Coupons:**
- Use clear, memorable codes
- Set appropriate limits
- Track usage and effectiveness
- Create time-limited offers
- Segment by user type

**Examples:**
- `WELCOME10` - 10% off for new users
- `HOLIDAY50` - 50% off holiday promotion
- `UPGRADE25` - 25% off plan upgrades

---

## Support Best Practices

### Response Guidelines

**First Response:**
1. Acknowledge receipt
2. Thank user for contacting support
3. Provide expected resolution time
4. Ask clarifying questions if needed
5. Set clear next steps

**Follow-Up:**
1. Update user on progress
2. Request additional information if needed
3. Provide interim solutions
4. Keep communication professional
5. Resolve or escalate promptly

### Escalation Process

**When to Escalate:**
- Technical issues beyond support scope
- Requests for refunds/exceptions
- Security or privacy concerns
- Complaints about service
- Unresolved after 48 hours

**Escalation Steps:**
1. Document issue thoroughly
2. Tag for supervisor review
3. Notify escalation team
4. Transfer ticket with context
5. Follow up on resolution

---

## Troubleshooting

### Cannot View Ticket

**Issue:** Ticket won't open or load

**Solutions:**
1. Refresh the page
2. Clear browser cache
3. Check permissions
4. Try different browser
5. Contact technical support

### Withdrawal Not Processing

**Issue:** Withdrawal stuck in pending

**Solutions:**
1. Verify bank details are correct
2. Check for sufficient balance
3. Confirm minimum payout met
4. Review for holds or restrictions
5. Process manually if needed

### Affiliate Link Not Working

**Issue:** Referral link returns error

**Solutions:**
1. Regenerate affiliate link
2. Check link format
3. Verify affiliate is active
4. Test in different browser
5. Clear tracking cookies

---

## Additional Resources

**Related Documentation:**
- [User Management](user-management.md) - Manage support ticket authors
- [Dashboard](dashboard.md) - Monitor support metrics
- [Reseller Management](reseller.md) - Handle reseller support

---

**Previous:** [← Announcements](announcements.md) | **Next:** [Reseller →](reseller.md)
