# SMS Marketing Setup Guide for Real Estate

## Overview
SMS marketing is one of the most effective channels for real estate - with 98% open rates and 45% response rates, it's perfect for urgent property alerts, appointment reminders, and time-sensitive offers. This guide shows you how to set up SMS marketing for Gippsland Property Sales.

**Note**: 
- **If you use @realty platform**: See `/sms-marketing/atrealty-sms-integration-guide.md` - Your platform already has SMS built-in!
- For Gippsland-specific SMS templates, see `/sms-marketing/gippsland-sms-templates.md`
- For King Kong methodology applied to SMS for appraisals, see `/sms-marketing/king-kong-sms-appraisal-strategy.md`

---

## Why SMS Marketing Works for Real Estate

### Key Benefits:
- **98% Open Rate**: People read SMS messages within 3 minutes
- **45% Response Rate**: Much higher than email (5-10%)
- **Immediate**: Perfect for time-sensitive property alerts
- **Personal**: Feels more direct and personal than email
- **Mobile-First**: Most property searches happen on mobile

### Best Use Cases:
- Property alerts (new listings matching criteria)
- Appointment reminders (appraisals, viewings)
- Urgent market updates
- Time-sensitive offers
- Follow-up after property viewings
- Re-engagement with cold leads

---

## Australian SMS Compliance (ACMA Rules)

**CRITICAL**: You MUST comply with Australian Communications and Media Authority (ACMA) rules:

### Key Requirements:
1. **Opt-In Required**: Must have explicit consent before sending marketing SMS
2. **Opt-Out Required**: Every SMS must include opt-out instructions (e.g., "Reply STOP to unsubscribe")
3. **Identify Yourself**: Must include your business name in every message
4. **Honour Opt-Outs**: Must remove from list within 5 business days
5. **No Spam**: Can only send to people who have consented

### How to Get Consent:
- ✅ Checkbox on landing page: "I consent to receive SMS updates"
- ✅ Form field: "Would you like SMS alerts? Yes/No"
- ✅ Verbal consent: "Can I send you SMS updates?"
- ✅ Double opt-in: Send confirmation SMS asking them to reply YES

### Penalties:
- Up to $1.1 million AUD per violation
- Individual fines up to $220,000 AUD
- Serious consequences - always get consent first!

---

## SMS Provider Options (Australian)

### Option 1: MessageMedia (Recommended for Australia)
**Best for**: Australian businesses, real estate, high volume

**Pricing**:
- Pay-as-you-go: ~$0.06-0.08 AUD per SMS
- Monthly plans: From $49/month (includes credits)
- Free trial: 100 free SMS

**Features**:
- Australian phone numbers
- Two-way messaging
- Automation workflows
- CRM integrations (HubSpot, Salesforce)
- Opt-out management (automatic)
- Delivery reports
- Short codes available

**Setup**:
1. Sign up at messagemedia.com.au
2. Verify your business (required for Australian SMS)
3. Get approved phone number
4. Set up automation workflows
5. Import contacts (with consent records)

**Pros**:
- Australian company, understands local compliance
- Excellent deliverability in Australia
- Good customer support
- Integrates with major CRMs

**Cons**:
- Slightly more expensive than some options
- Approval process can take 1-2 days

---

### Option 2: Twilio (International, Works in Australia)
**Best for**: Technical users, custom integrations

**Pricing**:
- Pay-as-you-go: ~$0.05-0.07 AUD per SMS
- No monthly fees
- Free trial: $15 USD credit

**Features**:
- API for custom integrations
- Two-way messaging
- Webhooks for automation
- Good documentation
- Works globally

**Setup**:
1. Sign up at twilio.com
2. Get Australian phone number
3. Set up API integration
4. Build automation (requires coding or Zapier)

**Pros**:
- Very flexible
- Good for developers
- Competitive pricing
- Reliable delivery

**Cons**:
- Requires technical knowledge or Zapier
- Less user-friendly interface
- Support can be slower

---

### Option 3: SMS Broadcast (Australian)
**Best for**: Small businesses, simple campaigns

**Pricing**:
- Pay-as-you-go: ~$0.05-0.07 AUD per SMS
- Monthly plans: From $29/month
- Free trial: 50 free SMS

**Features**:
- Simple interface
- Contact management
- Basic automation
- Opt-out management
- Australian support

**Setup**:
1. Sign up at smsbroadcast.com.au
2. Verify account
3. Upload contacts
4. Create campaigns

**Pros**:
- Easy to use
- Australian company
- Good for beginners
- Affordable

**Cons**:
- Limited automation features
- Fewer CRM integrations
- Less advanced than MessageMedia

---

### Option 4: SimpleTexting (US-based, Works in Australia)
**Best for**: Small businesses, simple automation

**Pricing**:
- Monthly plans: From $25 USD/month (500 SMS)
- Pay-as-you-go: ~$0.05 USD per SMS
- Free trial: 14 days

**Features**:
- Easy automation builder
- Keyword automation (e.g., "APPRAISAL" triggers sequence)
- Contact segmentation
- Basic CRM features
- Opt-out management

**Setup**:
1. Sign up at simpletexting.com
2. Get Australian phone number
3. Set up automation workflows
4. Import contacts

**Pros**:
- Very user-friendly
- Good automation features
- Affordable for small volume
- Good documentation

**Cons**:
- US company (support hours)
- Less Australian-specific features
- Phone number may be US-based

---

## Recommended Setup: MessageMedia

For Gippsland Property Sales, we recommend **MessageMedia** because:
- Australian company (better compliance support)
- Excellent deliverability in Australia
- Good automation features
- CRM integrations available
- Professional appearance (Australian phone numbers)

---

## Quick Start Checklist

- [ ] Choose SMS provider (MessageMedia recommended)
- [ ] Sign up and verify business account
- [ ] Get approved phone number
- [ ] Set up opt-in process on landing pages
- [ ] Create SMS templates (see templates file)
- [ ] Set up automation workflows
- [ ] Import contacts (with consent records)
- [ ] Test send to yourself
- [ ] Launch first campaign
- [ ] Monitor opt-outs and engagement

---

## Integration with Landing Pages

### Add SMS Opt-In to Your Forms

**Example Checkbox**:
```html
<div class="sms-opt-in">
  <label>
    <input type="checkbox" name="sms_consent" value="yes" required>
    I consent to receive SMS updates about properties and market information. 
    Reply STOP to unsubscribe. Message and data rates may apply.
  </label>
</div>
```

**Example Radio Buttons**:
```html
<div class="sms-opt-in">
  <p>Would you like SMS alerts for new properties?</p>
  <label>
    <input type="radio" name="sms_alerts" value="yes">
    Yes, send me SMS alerts
  </label>
  <label>
    <input type="radio" name="sms_alerts" value="no" checked>
    No, email only
  </label>
</div>
```

### Store Consent in CRM

When form is submitted:
1. ✅ Check if SMS consent is given
2. ✅ Store consent date and method in CRM
3. ✅ Add to SMS marketing list
4. ✅ Send welcome SMS (if opted in)

---

## Integration with CRM

### Google Sheets Integration:

Add SMS columns to your lead tracking sheet:
- **SMS Consent**: Yes/No
- **SMS Opt-In Date**: Date they consented
- **SMS Status**: Active/Unsubscribed/Not Opted In
- **Last SMS Sent**: Date of last message
- **SMS Engagement**: Opened/Clicked/Replied

### HubSpot Integration:

1. Create custom property: "SMS Consent"
2. Create custom property: "SMS Opt-In Date"
3. Use HubSpot workflows to:
   - Add to SMS list when consent given
   - Remove from SMS list when unsubscribed
   - Track SMS engagement

### MessageMedia CRM Integration:

MessageMedia integrates with:
- HubSpot
- Salesforce
- Zoho CRM
- Custom API integrations

**Setup**:
1. Connect MessageMedia to your CRM
2. Sync contacts automatically
3. Track SMS engagement in CRM
4. Trigger SMS from CRM actions

---

## SMS Best Practices

### Message Length:
- **Keep it short**: 160 characters or less (one SMS)
- **Be concise**: Get to the point quickly
- **Include value**: Why are you messaging them?

### Timing:
- **Best times**: 9am-12pm, 2pm-5pm (weekdays)
- **Avoid**: Before 8am, after 8pm, weekends (unless urgent)
- **Property alerts**: Can send anytime (high value)

### Frequency:
- **Don't overdo it**: 2-4 SMS per month maximum
- **Only send value**: Property alerts, appointments, urgent updates
- **Respect opt-outs**: Remove immediately when requested

### Personalisation:
- ✅ Use their name: "Hi [Name],"
- ✅ Reference their interest: "New property in [Suburb]"
- ✅ Include your name: "From [Your Name]"

### Call-to-Action:
- ✅ Clear action: "Reply YES to schedule"
- ✅ Include link: "View property: [short link]"
- ✅ Make it easy: "Call me: [phone number]"

### Compliance:
- ✅ Always include opt-out: "Reply STOP to unsubscribe"
- ✅ Include business name: "@realty Property Sales Gippsland"
- ✅ Only send to opted-in contacts

---

## Automation Workflows

### Workflow 1: Welcome SMS (Immediate)
**Trigger**: New lead opts in for SMS
**Message**: Welcome message + what to expect
**Timing**: Send immediately

### Workflow 2: Appointment Reminder (24 hours before)
**Trigger**: Appointment scheduled in CRM
**Message**: Reminder with date/time/address
**Timing**: 24 hours before appointment

### Workflow 3: Property Alert (When new listing matches)
**Trigger**: New property matches their criteria
**Message**: Property details + link
**Timing**: Send within 1 hour of listing

### Workflow 4: Follow-Up After Viewing (Same day)
**Trigger**: Property viewing completed
**Message**: "How did you like the property?"
**Timing**: Same day, 2-4 hours after viewing

### Workflow 5: Market Update (Monthly)
**Trigger**: Monthly automation
**Message**: Gippsland market update
**Timing**: First Monday of each month

### Workflow 6: Re-engagement (30 days inactive)
**Trigger**: No engagement for 30 days
**Message**: "Still looking? New properties available"
**Timing**: 30 days after last contact

---

## Cost Comparison

| Solution | King Kong | DIY (MessageMedia) |
|----------|-----------|-------------------|
| SMS Platform | Included | $49-99/month |
| SMS Credits | Included | ~$0.06-0.08 per SMS |
| Automation | Included | Included (free) |
| CRM Integration | Included | Included (free) |
| **Total** | **$18,000** | **~$100-200/month** |

**Monthly Cost Estimate**:
- 500 SMS/month = ~$30-40 in credits
- Platform fee = $49/month
- **Total: ~$80-90/month**

---

## Next Steps

1. **Choose Provider**: Sign up with MessageMedia (recommended)
2. **Get Approved**: Complete business verification
3. **Set Up Opt-In**: Add SMS consent to landing pages
4. **Create Templates**: See `/sms-marketing/gippsland-sms-templates.md`
5. **Set Up Automation**: Configure workflows
6. **Import Contacts**: Add opted-in contacts
7. **Test**: Send test messages to yourself
8. **Launch**: Start with welcome SMS to new leads

---

## Resources

- **ACMA Spam Rules**: https://www.acma.gov.au/spam-rules
- **MessageMedia**: https://www.messagemedia.com.au
- **Twilio**: https://www.twilio.com
- **SMS Broadcast**: https://www.smsbroadcast.com.au

---

## Support

If you need help:
1. Check provider documentation
2. Review compliance requirements
3. Test with small groups first
4. Monitor opt-out rates (should be <1%)

Remember: SMS is powerful but must be used responsibly. Always get consent, always include opt-out, and always provide value!

