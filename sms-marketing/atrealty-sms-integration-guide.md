# @realty SMS Marketing Integration Guide

## Overview
Your @realty platform already has SMS marketing built-in and integrated with your CRM database. This guide shows you how to use it effectively to generate property appraisals using King Kong's direct response methodology.

**Access**: `myatrealty.com/agent/marketing?product=sms-marketing`

---

## Understanding Your @realty SMS Marketing System

### What You Have:
- ✅ **Built-in SMS Platform**: No need for external providers (MessageMedia, etc.)
- ✅ **CRM Integration**: All your contacts are already in the system
- ✅ **Campaign Management**: Create, schedule, and track SMS campaigns
- ✅ **Recipient Management**: Select contacts from your database
- ✅ **Template System**: Save and reuse SMS templates
- ✅ **Status Tracking**: See which campaigns are draft, sent, or scheduled
- ✅ **Unsubscribed Management**: Track opt-outs automatically

### What You Can Do:
1. **Create SMS Campaigns**: Send to selected contacts
2. **Use Templates**: Save time with reusable templates
3. **Schedule Campaigns**: Set launch dates for future sends
4. **Track Recipients**: See how many people received each campaign
5. **Manage Opt-Outs**: Handle unsubscribes automatically

---

## How to Use @realty SMS for Appraisal Generation

### Step 1: Access SMS Marketing

1. Log into @realty platform: `myatrealty.com`
2. Navigate to: **Marketing** → **SMS Marketing**
3. You'll see:
   - **Campaigns Tab**: Your active campaigns
   - **Unsubscribed Tab**: People who opted out
   - **Create SMS Marketing Campaign** button

---

### Step 2: Create Your First Appraisal Campaign

#### Campaign Setup:

1. **Click "Create SMS Marketing Campaign"**
2. **Campaign Name**: 
   - Use descriptive names like:
     - "Appraisal Welcome - [Date]"
     - "Market Update - [Suburb] - [Date]"
     - "Appointment Reminder - [Date]"
3. **Select Recipients**:
   - Choose contacts from your CRM database
   - Filter by:
     - Contact type (leads, clients, etc.)
     - Suburb (Drouin, Trafalgar, Warragul, etc.)
     - Status (new leads, appraisal requested, etc.)
     - Date added (recent leads, etc.)
4. **Create Message**:
   - Write your SMS (or use template)
   - Character limit: 160 characters (one SMS)
   - Longer messages will split into multiple SMS (costs more)
5. **Choose Template** (optional):
   - Save message as template for reuse
6. **Set Launch Date**:
   - Send immediately, or schedule for later
7. **Review & Send**:
   - Preview message
   - Check recipient count
   - Launch campaign

---

## King Kong Methodology Applied to @realty SMS

### Principle 1: Direct Response (Clear Call-to-Action)

**Every SMS must have a clear action:**

**Template Structure**:
```
[Greeting] [Value/Message] [Action] [Compliance]
```

**Example**:
```
Hi [Name]! Free property appraisal in [Suburb]. 
Reply YES or call 0409 183 763. Reply STOP to opt out. 
@realty Gippsland
```

**Breakdown**:
- **Greeting**: "Hi [Name]!" (personal)
- **Value**: "Free property appraisal in [Suburb]" (benefit)
- **Action**: "Reply YES or call 0409 183 763" (clear CTA)
- **Compliance**: "Reply STOP to opt out" (required)
- **Branding**: "@realty Gippsland" (identify yourself)

---

### Principle 2: Segment Your Contacts

**Create Segments for Targeted Campaigns:**

#### Segment 1: New Appraisal Leads
- **Who**: People who requested appraisal in last 7 days
- **Campaign**: Welcome SMS + Value content
- **Goal**: Confirm interest, set expectations

#### Segment 2: Appraisal Scheduled
- **Who**: People with appraisal appointments
- **Campaign**: Reminder SMS (24hrs before)
- **Goal**: Reduce no-shows

#### Segment 3: Post-Appraisal Follow-Up
- **Who**: People who had appraisal in last 3 days
- **Campaign**: Thank you + Report delivery
- **Goal**: Maintain engagement, move toward listing

#### Segment 4: Cold Leads (30+ days)
- **Who**: People who requested appraisal but haven't responded
- **Campaign**: Re-engagement SMS
- **Goal**: Re-activate interest

#### Segment 5: Active Buyers
- **Who**: People looking to buy properties
- **Campaign**: New property alerts
- **Goal**: Show relevant properties

---

### Principle 3: Create SMS Templates

**Save Templates for Quick Use:**

#### Template 1: Appraisal Welcome
```
Hi [Name]! Thanks for requesting your free property 
appraisal in [Suburb]. Mel or Jeff will contact you 
within 24hrs. Questions? Call 0409 183 763. Reply 
STOP to opt out. @realty Gippsland
```

#### Template 2: Appointment Reminder
```
Hi [Name]! Reminder: Your property appraisal tomorrow 
[Date] at [Time] at [Address]. See you then! Reply 
STOP to opt out. @realty Gippsland
```

#### Template 3: Market Update
```
[Name], [X] properties sold in [Suburb] this month. 
Avg price $[X]. Ready for your free appraisal? Reply 
YES or call 0409 183 763. Reply STOP to opt out. 
@realty Gippsland
```

#### Template 4: Post-Appraisal Follow-Up
```
Hi [Name]! Thanks for your time today. Your property 
valuation report will be emailed within 24hrs. 
Questions? Call 0409 183 763. Reply STOP to opt out. 
@realty Gippsland
```

#### Template 5: Re-engagement
```
[Name], still curious about your [Suburb] property 
value? Free appraisal available. No obligation. 
Reply YES or call 0409 183 763. Reply STOP to opt 
out. @realty Gippsland
```

**How to Save Templates in @realty**:
1. Create campaign message
2. Look for "Save as Template" option
3. Name your template (e.g., "Appraisal Welcome")
4. Use template for future campaigns

---

### Principle 4: Automation Workflows

**Set Up Regular Campaigns:**

#### Workflow 1: New Lead Welcome (Daily)
- **Trigger**: New contact added with "Appraisal Requested" status
- **Action**: Send welcome SMS within 1 hour
- **Template**: Appraisal Welcome
- **Recipients**: Filter by status = "New Lead" + Date = Today

#### Workflow 2: Appointment Reminders (Daily)
- **Trigger**: Appraisal scheduled for tomorrow
- **Action**: Send reminder SMS 24 hours before
- **Template**: Appointment Reminder
- **Recipients**: Filter by status = "Appraisal Scheduled" + Date = Tomorrow

#### Workflow 3: Market Update (Weekly)
- **Trigger**: Every Monday morning
- **Action**: Send market update to all active leads
- **Template**: Market Update (customise with current data)
- **Recipients**: Filter by status = "Active Lead" + Last contact < 30 days

#### Workflow 4: Re-engagement (Monthly)
- **Trigger**: First Monday of each month
- **Action**: Send re-engagement SMS to cold leads
- **Template**: Re-engagement
- **Recipients**: Filter by status = "Cold Lead" + Last contact > 30 days

**Note**: @realty may have automation features. Check "Setup" or contact @realty support to see if you can automate these workflows. If not, set up manual reminders to create these campaigns regularly.

---

## Complete SMS Campaign Strategy for Appraisals

### Campaign 1: Welcome SMS (Immediate)

**When to Send**: Within 1 hour of form submission

**Recipients**: 
- New contacts with "Appraisal Requested" status
- Added in last 24 hours

**Message**:
```
Hi [Name]! Thanks for requesting your free property 
appraisal in [Suburb]. Mel or Jeff will contact you 
within 24hrs. Get your free [Suburb] market report: 
[Link]. Reply STOP to opt out. @realty Gippsland
```

**Goal**: Confirm receipt, set expectations, provide value

---

### Campaign 2: Appointment Confirmation (After Scheduling)

**When to Send**: Immediately after appraisal scheduled

**Recipients**: 
- Contacts with "Appraisal Scheduled" status
- Appraisal date = next 7 days

**Message**:
```
Hi [Name]! Your appraisal confirmed: [Date] at [Time] 
at [Address]. Mel/Jeff will bring market analysis for 
[Suburb]. See you then! Reply STOP to opt out. 
@realty Gippsland
```

**Goal**: Confirm appointment, reduce no-shows

---

### Campaign 3: Appointment Reminder (24 Hours Before)

**When to Send**: 24 hours before appointment

**Recipients**: 
- Contacts with appraisal scheduled for tomorrow
- Status = "Appraisal Scheduled"

**Message**:
```
Hi [Name]! Reminder: Your property appraisal tomorrow 
[Date] at [Time] at [Address]. See you then! Reply 
STOP to opt out. @realty Gippsland
```

**Goal**: Reduce no-shows, show professionalism

---

### Campaign 4: Market Update (Day 5 - If No Response)

**When to Send**: 5 days after initial contact, if no response

**Recipients**: 
- Contacts with "Appraisal Requested" status
- Last contact = 5 days ago
- No appointment scheduled

**Message**:
```
[Name], Gippsland market update: [X] properties sold 
in [Suburb] this month. Avg price $[X]. Still 
interested in your free appraisal? Reply YES or call 
0409 183 763. Reply STOP to opt out. @realty Gippsland
```

**Goal**: Re-engage, provide value, encourage action

---

### Campaign 5: Post-Appraisal Follow-Up (Same Day)

**When to Send**: 2-4 hours after appraisal completed

**Recipients**: 
- Contacts with "Appraisal Completed" status
- Appraisal date = today

**Message**:
```
Hi [Name]! Thanks for your time today. Your property 
valuation report will be emailed within 24hrs. 
Questions? Call 0409 183 763. Reply STOP to opt out. 
@realty Gippsland
```

**Goal**: Maintain engagement, open door for listing conversation

---

### Campaign 6: Re-engagement (Day 30)

**When to Send**: 30 days after initial contact, if no engagement

**Recipients**: 
- Contacts with "Appraisal Requested" status
- Last contact > 30 days ago
- No appointment scheduled

**Message**:
```
[Name], still curious about your [Suburb] property 
value? Free appraisal available. No obligation. Reply 
YES or call 0409 183 763. Reply STOP to opt out. 
@realty Gippsland
```

**Goal**: Re-activate cold leads

---

## How to Segment Contacts in @realty

### Using Contact Filters:

When creating a campaign, you'll see options to filter recipients:

1. **By Status**:
   - New Lead
   - Appraisal Requested
   - Appraisal Scheduled
   - Appraisal Completed
   - Active Lead
   - Cold Lead

2. **By Suburb**:
   - Drouin
   - Trafalgar
   - Warragul
   - Moe
   - Traralgon
   - Other

3. **By Date**:
   - Added in last 7 days
   - Added in last 30 days
   - Last contact date

4. **By Property Type**:
   - House
   - Unit
   - Townhouse
   - Land
   - Commercial

**Best Practice**: Create segments by combining filters:
- Example: "New Appraisal Leads" = Status = "Appraisal Requested" + Date Added = Last 7 days

---

## Integration with Your Marketing Funnel

### How SMS Fits into Your Existing Funnel:

**Current Funnel**:
```
Ad → Landing Page → Form → Email → CRM → Call → Appraisal
```

**Enhanced Funnel (with SMS)**:
```
Ad → Landing Page → Form → SMS + Email → CRM → Call → Appraisal
```

### Integration Points:

1. **Landing Page Form**:
   - Add SMS opt-in checkbox: "I consent to receive SMS updates"
   - When form submitted → Contact added to @realty CRM
   - Status set to "Appraisal Requested"
   - Trigger welcome SMS campaign

2. **Email Automation**:
   - SMS works alongside email
   - Email for longer content
   - SMS for urgent/action-oriented messages
   - Multi-channel = higher engagement

3. **CRM Updates**:
   - When contact responds to SMS → Update status in @realty CRM
   - When appointment scheduled → Update status → Trigger reminder SMS
   - Track SMS engagement in contact notes

---

## Best Practices for @realty SMS

### Message Guidelines:

1. **Keep It Short**: Under 160 characters when possible
2. **Be Personal**: Use [Name] and [Suburb] when available
3. **Clear Action**: "Reply YES", "Call [Phone]", "View: [Link]"
4. **Provide Value**: Why are you messaging them?
5. **Compliance**: Always include "Reply STOP to opt out"
6. **Branding**: Include "@realty Gippsland" or business name

### Timing Guidelines:

- **Best Times**: 9am-12pm, 2pm-5pm (weekdays)
- **Avoid**: Before 8am, after 8pm, weekends (unless urgent)
- **Property Alerts**: Can send anytime (high value)
- **Appointments**: 24 hours before is ideal

### Frequency Guidelines:

- **Maximum**: 2-4 SMS per month per contact
- **Property Alerts**: Unlimited (they opted in for this)
- **Nurture Sequence**: 1-2 per week maximum
- **Transactional**: As needed (appointments, reminders)

---

## Tracking & Analytics

### Metrics to Track in @realty:

1. **Recipient Count**: How many people received SMS
2. **Response Rate**: How many replied (track manually in CRM notes)
3. **Appointment Booking Rate**: How many booked after SMS
4. **Cost per SMS**: Check with @realty for pricing
5. **Opt-Out Rate**: Monitor unsubscribes (should be <1%)

### How to Track:

1. **In @realty CRM**:
   - Add notes when contact responds to SMS
   - Update status when action taken
   - Track appointment bookings

2. **Manual Tracking**:
   - Create spreadsheet to track:
     - Campaign name
     - Date sent
     - Recipients
     - Responses
     - Appointments booked
     - Cost

3. **Review Weekly**:
   - Which campaigns got best response?
   - Which messages converted to appointments?
   - What time of day works best?
   - Optimise based on data

---

## Cost Considerations

### @realty SMS Pricing:

Check with @realty support for:
- Cost per SMS
- Monthly plans
- Volume discounts
- Included credits

**Typical SMS Costs**:
- ~$0.05-0.08 AUD per SMS in Australia
- Monthly platform fees may apply
- Check your @realty agreement

**Cost Estimate** (if paying per SMS):
- 100 new leads/month × 3 SMS = 300 SMS
- 50 appointment reminders = 50 SMS
- 30 follow-ups = 30 SMS
- **Total: ~400 SMS/month**
- **Cost: ~$20-32/month** (at $0.05-0.08 per SMS)

---

## Quick Start Checklist

### Week 1: Setup
- [ ] Access @realty SMS Marketing section
- [ ] Review existing contacts in CRM
- [ ] Create contact segments (new leads, scheduled, etc.)
- [ ] Create SMS templates (use templates in this guide)
- [ ] Test send SMS to yourself

### Week 2: Launch
- [ ] Create welcome SMS campaign for new leads
- [ ] Create appointment reminder campaign
- [ ] Send first campaign to test group
- [ ] Monitor responses
- [ ] Track metrics

### Week 3: Optimize
- [ ] Review response rates
- [ ] A/B test different messages
- [ ] Optimize send times
- [ ] Improve templates
- [ ] Scale successful campaigns

---

## Troubleshooting

### Common Issues:

**Q: Can't find SMS Marketing section?**
- Check with @realty support
- May need to enable feature
- Check user permissions

**Q: Can't select recipients?**
- Check contact filters
- Ensure contacts have phone numbers
- Check contact status

**Q: Messages not sending?**
- Check launch date (may be scheduled)
- Check recipient count (may be 0)
- Contact @realty support

**Q: Need automation?**
- Check if @realty has automation features
- If not, set up manual reminders
- Consider using Zapier (if @realty integrates)

---

## Next Steps

1. **Access Your SMS Marketing**: Log into @realty and navigate to SMS Marketing
2. **Review Contacts**: See what contacts you have available
3. **Create Templates**: Save the templates from this guide
4. **Create First Campaign**: Start with welcome SMS for new leads
5. **Track Results**: Monitor responses and appointments booked
6. **Optimize**: Improve based on data

---

## Integration with Other Marketing

### Connect SMS to:

1. **Landing Pages**:
   - Add SMS opt-in checkbox
   - Form submissions → @realty CRM → SMS campaign

2. **Email Automation**:
   - SMS for urgent messages
   - Email for longer content
   - Multi-channel approach

3. **Google Ads / Facebook Ads**:
   - Track which ads generate SMS-engaged leads
   - Optimize ads based on SMS response rates

4. **CRM Workflow**:
   - Status changes → Trigger SMS campaigns
   - Appointment scheduled → Reminder SMS
   - Appraisal completed → Follow-up SMS

---

## Key Takeaways

1. **You Already Have It**: @realty SMS is built-in, no external provider needed
2. **CRM Integration**: All contacts are already in the system
3. **King Kong Methodology**: Apply direct response principles to SMS
4. **Segment Contacts**: Target messages to specific groups
5. **Use Templates**: Save time with reusable templates
6. **Track Everything**: Monitor responses and optimize
7. **Multi-Channel**: SMS + Email = Higher engagement

---

*Your @realty platform already has everything you need for SMS marketing. Apply King Kong's methodology and watch your appraisal bookings increase!*

