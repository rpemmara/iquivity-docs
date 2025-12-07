# Troubleshooting Common Issues

Solutions to common problems and issues you may encounter while using iQuivity AI.

## Content Generation Issues

### Issue: Content Generation Fails

**Symptoms:**
- Error message when generating content
- Request times out
- No response received

**Common Causes & Solutions:**

**1. Insufficient Credits**

Check your credit balance:
```
Dashboard → Usage Statistics → Credits Remaining
```

**Solution:**
- Upgrade your plan
- Purchase additional credits
- Wait for monthly credit reset

**2. Network/Connectivity Issues**

**Solution:**
- Check your internet connection
- Try refreshing the page
- Clear browser cache
- Try a different browser

**3. Prompt Too Complex**

**Solution:**
- Simplify your prompt
- Break into smaller requests
- Reduce word count requirement
- Lower creativity setting

**4. Service Temporarily Down**

**Solution:**
- Check status page: https://status.iquivity.ai
- Wait a few minutes and retry
- Contact support if persistent

### Issue: Poor Quality Output

**Symptoms:**
- Generated content doesn't match expectations
- Off-topic or irrelevant content
- Grammatical errors
- Incomplete responses

**Solutions:**

**1. Improve Your Prompt**

❌ **Vague:**
```
"Write about marketing"
```

✅ **Specific:**
```
"Write a 500-word blog post about email marketing best practices
for small businesses, using a friendly and professional tone,
including 3 actionable tips with examples."
```

**2. Adjust Settings**
- Change tone (professional, casual, friendly)
- Modify creativity level
- Specify target audience
- Set appropriate length

**3. Use Templates**
- Browse template library
- Choose relevant template
- Provides better structure

**4. Iterate and Refine**
- Generate initial version
- Use "Improve" feature
- Regenerate specific sections
- Add more context if needed

### Issue: Generation Takes Too Long

**Symptoms:**
- Processing for more than 2 minutes
- Page appears stuck
- No progress indication

**Solutions:**

**1. Reduce Complexity**
- Shorten requested length
- Use lower quality settings (for images)
- Simplify requirements

**2. Check Plan Limits**
- Free/Starter plans may have slower processing
- Upgrade to Professional for priority processing
- Enterprise gets fastest processing

**3. Try During Off-Peak Hours**
- High traffic times may be slower
- Try early morning or late evening

**4. Clear and Retry**
- Cancel current request
- Start fresh request
- Sometimes resolves stuck requests

## File Upload Issues

### Issue: Files Won't Upload

**Symptoms:**
- Upload fails with error
- Progress bar stuck
- "Upload failed" message

**Common Causes & Solutions:**

**1. File Too Large**

Check file size limits:
- **Free:** 25 MB max
- **Starter:** 100 MB max
- **Professional:** 500 MB max
- **Enterprise:** 2 GB max

**Solution:**
- Compress file
- Split into smaller files
- Upgrade plan for larger limits

**2. Unsupported Format**

**Solution:**
- Convert to supported format
- Check file extension
- Contact support for format questions

**3. Storage Full**

**Solution:**
```
Settings → Storage → View Usage
```
- Delete old files
- Empty trash
- Upgrade storage plan

**4. Browser Issues**

**Solution:**
- Clear browser cache and cookies
- Try different browser (Chrome, Firefox, Safari)
- Disable browser extensions
- Update browser to latest version

**5. Network Issues**

**Solution:**
- Check internet connection
- Try on different network
- Wait and retry during better connection
- Use wired connection if on WiFi

### Issue: Uploaded Files Not Appearing

**Symptoms:**
- Upload completes successfully
- File doesn't show in file list
- Can't find uploaded file

**Solutions:**

**1. Refresh the Page**
- Press F5 or Cmd+R
- Hard refresh: Ctrl+Shift+R (Cmd+Shift+R on Mac)

**2. Check Filters**
- Clear all active filters
- Check "All Files" view
- Search by filename

**3. Check Folder Location**
- Verify upload destination folder
- Check if in different folder

**4. Processing Delay**
- Large files may take time to process
- Check back in a few minutes
- Receive email when complete

## Chatbot Issues

### Issue: Chatbot Not Responding

**Symptoms:**
- No response to messages
- "Chatbot unavailable" error
- Loading indicator stuck

**Solutions:**

**1. Check Chatbot Status**
```
Dashboard → Chatbots → [Your Chatbot] → Settings
```
- Verify chatbot is "Active"
- Check operating hours
- Ensure not paused

**2. Verify Embed Code**

**For Website Integration:**
- Check embed code is correct
- Verify placed before `</body>` tag
- Check for JavaScript errors (browser console)
- Ensure chatbot ID is correct

**3. Test in Dashboard**
- Go to chatbot testing interface
- Test with sample questions
- If works there, issue is with deployment

**4. Check Training Data**
- Verify chatbot has training data
- Re-index training content
- Add more training if limited

**5. Clear Browser Data**
- Clear cache and cookies
- Try incognito/private mode
- Test in different browser

### Issue: Chatbot Gives Wrong Answers

**Symptoms:**
- Incorrect or irrelevant responses
- Out-of-date information
- Doesn't understand questions

**Solutions:**

**1. Review Training Data**
- Check if relevant information exists
- Update outdated content
- Add missing information
- Remove conflicting data

**2. Add Question Variations**
- Include alternative phrasings
- Add synonyms
- Cover common variations

**3. Improve Training Quality**
- Use clear, well-structured content
- Avoid duplicate information
- Organize by topic
- Use consistent terminology

**4. Adjust Confidence Threshold**
```
Chatbot Settings → Behavior → Confidence Threshold
```
- Increase threshold for more accuracy
- May trigger more fallbacks
- Find balance for your use case

**5. Test and Iterate**
- Test with real user questions
- Review unanswered queries
- Continuously improve training

### Issue: Chatbot Widget Not Displaying

**Symptoms:**
- Chat widget doesn't appear on website
- Only shows briefly then disappears
- Appears but non-functional

**Solutions:**

**1. Verify Installation**
```html
<!-- Check this code is on your website -->
<script src="https://iquivity.ai/chatbot-embed.js"></script>
<script>
  ChatBot.init({
    chatbotId: 'your-chatbot-id' // Verify ID is correct
  });
</script>
```

**2. Check for Conflicts**
- Other chat widgets may conflict
- Disable other scripts temporarily
- Check browser console for errors

**3. Verify Domain**
- Some chatbots may be domain-restricted
- Check allowed domains in settings
- Add your domain if needed

**4. Check CSS Conflicts**
- Your site CSS may hide widget
- Check z-index settings
- Inspect element in browser dev tools

**5. Test Different Browsers**
- May be browser-specific issue
- Test Chrome, Firefox, Safari
- Check mobile browsers

## Account Access Issues

### Issue: Can't Log In

**Symptoms:**
- "Invalid email or password" error
- Account locked message
- Can't receive verification code

**Solutions:**

**1. Verify Credentials**
- Check email address is correct
- Verify caps lock is off
- Try copying/pasting password
- Check for extra spaces

**2. Reset Password**
```
Login Page → "Forgot Password?"
```
- Enter registered email
- Check inbox (and spam folder)
- Follow reset link
- Create new password

**3. 2FA Issues**
- Verify code from authenticator app
- Ensure device time is synced
- Use backup code if available
- Disable and re-enable 2FA if needed

**4. Account Locked**
- After multiple failed attempts
- Wait 30 minutes
- Contact support@iquivity.ai

**5. Email Not Verified**
- Check for verification email
- Resend verification email
- Check spam/junk folder
- Add noreply@iquivity.ai to contacts

### Issue: Missing Features/Content

**Symptoms:**
- Features you had access to are gone
- Can't see previously created content
- Missing team members or chatbots

**Possible Causes:**

**1. Plan Downgrade**
- Check current plan: Settings → Billing
- Some features require higher plans
- Upgrade to restore access

**2. Subscription Expired**
- Check billing status
- Update payment method
- Renew subscription

**3. Wrong Account**
- May be logged into different account
- Check email address in profile
- Switch accounts if multiple

**4. Accidental Deletion**
- Check trash folder
- Items kept for 30 days
- Restore from trash

**5. Team Settings Changed**
- For team accounts, permissions may have changed
- Contact team admin
- Verify your role and permissions

## Payment & Billing Issues

### Issue: Payment Failed

**Symptoms:**
- "Payment declined" error
- Unable to upgrade plan
- Subscription cancelled

**Solutions:**

**1. Verify Payment Method**
```
Settings → Billing → Payment Methods
```
- Check card is not expired
- Verify billing address is correct
- Ensure sufficient funds
- Update payment information

**2. Try Different Payment Method**
- Add new credit card
- Try PayPal
- Contact bank about international transactions

**3. Contact Support**
- If payment should have worked
- Provide transaction details
- Alternative payment arrangements

### Issue: Incorrect Charges

**Symptoms:**
- Unexpected charge
- Wrong amount billed
- Charged after cancellation

**Solutions:**

**1. Review Invoice**
```
Settings → Billing → Invoice History
```
- Check invoice details
- Verify services purchased
- Look for add-ons or overages

**2. Check Subscription Status**
- Verify plan and billing cycle
- Check if annual vs monthly
- Review any mid-cycle changes

**3. Contact Billing Support**
- Email: billing@iquivity.ai
- Include invoice number
- Describe discrepancy
- Request review

## Performance Issues

### Issue: Slow Performance

**Symptoms:**
- Pages load slowly
- Actions take long to complete
- Interface feels sluggish

**Solutions:**

**1. Browser Optimization**
- Clear cache and cookies
- Close unnecessary tabs
- Update browser to latest version
- Try different browser

**2. Internet Connection**
- Test connection speed
- Try wired connection
- Restart router
- Contact ISP if persistent

**3. Disable Extensions**
- Some extensions slow performance
- Try incognito/private mode
- Disable extensions one by one

**4. Check System Resources**
- Close other applications
- Check CPU/RAM usage
- Restart computer if needed

## API Issues

### Issue: API Requests Failing

**Symptoms:**
- 401 Unauthorized error
- 429 Rate Limit error
- 500 Server error

**Solutions:**

**1. 401 Unauthorized**
```json
{
  "error": {
    "code": "invalid_api_key"
  }
}
```

**Fix:**
- Verify API key is correct
- Check Authorization header format
- Regenerate API key if needed
- Ensure key hasn't been deleted

**2. 429 Rate Limit**
```json
{
  "error": {
    "code": "rate_limit_exceeded"
  }
}
```

**Fix:**
- Wait for rate limit to reset
- Implement exponential backoff
- Check rate limit headers
- Upgrade plan for higher limits
- Contact support for custom limits

**3. 500 Server Error**

**Fix:**
- Check status page
- Retry request after delay
- Contact support if persistent
- Implement retry logic

## Getting Additional Help

If you can't resolve your issue:

### 1. Search Documentation
- Use search bar at top
- Browse relevant sections
- Check FAQ

### 2. Check Status Page
- Visit: https://status.iquivity.ai
- See if there are known issues
- Subscribe to status updates

### 3. Community Forum
- Search existing topics
- Ask the community
- Share experiences

### 4. Contact Support
- See: [Contact Support](contact.md)
- Provide detailed information
- Include screenshots if relevant
- Specify steps to reproduce

### Information to Include

When contacting support, please provide:

- ✅ Account email address
- ✅ Plan type
- ✅ Detailed description of issue
- ✅ Steps to reproduce
- ✅ Screenshots or screen recordings
- ✅ Browser and version
- ✅ Operating system
- ✅ When issue started
- ✅ Any error messages
- ✅ What you've already tried

---

**Previous:** [← Billing & Subscription](../account/billing.md) | **Next:** [Best Practices →](best-practices.md)
