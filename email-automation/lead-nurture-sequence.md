# Email Automation Sequence for Real Estate Leads

## Overview
This is a 7-email sequence designed to nurture real estate leads from initial contact to closing. Each email is sent automatically based on lead behavior and timing.

**Note**: For Gippsland Property Sales, see `/email-automation/gippsland-email-templates.md` for Gippsland-specific, appraisal-focused email templates with Australian English and local market content.

## Setup Instructions

### Option 1: Mailchimp (Free up to 500 contacts)
1. Sign up at mailchimp.com
2. Create an automation workflow
3. Import these email templates
4. Set up triggers (form submission, time delays)

### Option 2: SendGrid (Free up to 100 emails/day)
1. Sign up at sendgrid.com
2. Create a dynamic template
3. Use their API to send emails

### Option 3: ConvertKit (Free up to 1,000 subscribers)
1. Sign up at convertkit.com
2. Create automation sequences
3. Import these templates

---

## Email Sequence

### Email 1: Welcome Email (Immediate)
**Subject:** Welcome! Let's Find Your Dream Home 🏠

**Body:**
```
Hi [Name],

Thank you for reaching out! I'm excited to help you [buy/sell] your perfect property.

As your real estate agent, I'll provide:
✓ Personalized property recommendations
✓ Market insights and pricing strategies
✓ Expert negotiation on your behalf
✓ Smooth transaction process

What happens next?
1. I'll review your preferences
2. Schedule a quick call to understand your needs
3. Start showing you properties that match your criteria

Would you prefer a call or email? Just reply to this message!

Best regards,
[Your Name]
[Your Business]
[Phone Number]
[Email]
```

---

### Email 2: Value Content (Day 2)
**Subject:** 5 Things Every Home Buyer Should Know

**Body:**
```
Hi [Name],

Before we start your home search, here are 5 crucial things every buyer should know:

1. **Get Pre-Approved First**
   - Know your budget before you fall in love with a home
   - Makes you a stronger buyer in competitive markets

2. **Location Matters More Than Size**
   - A smaller home in a great location often appreciates faster
   - Consider schools, commute, and neighborhood trends

3. **Don't Skip the Inspection**
   - Hidden issues can cost thousands later
   - Negotiate repairs or price adjustments

4. **Understand Market Conditions**
   - Seller's market = act fast, be competitive
   - Buyer's market = more negotiating power

5. **Work With a Local Expert**
   - Local knowledge = better deals and insights
   - That's where I come in! 😊

Ready to start? Let's schedule a call this week.

[Schedule Call Button/Link]

Best,
[Your Name]
```

---

### Email 3: Market Update (Day 5)
**Subject:** [Your City] Real Estate Market Update

**Body:**
```
Hi [Name],

Here's what's happening in the [Your City] real estate market this month:

📊 **Market Stats:**
- Average Days on Market: [X] days
- Median Home Price: $[X]
- Inventory: [X] homes available
- Price Trend: [Up/Down/Stable] [X]% from last month

💡 **What This Means for You:**
[Personalized insight based on their property type selection]

🏡 **Hot Properties This Week:**
[Link to 3-5 featured properties matching their criteria]

Want to see any of these in person? Just reply and I'll schedule a showing!

Best,
[Your Name]

P.S. New listings come in daily. Want me to send you alerts for properties matching your criteria?
```

---

### Email 4: Social Proof (Day 8)
**Subject:** How We Helped [Similar Client] Find Their Dream Home

**Body:**
```
Hi [Name],

I wanted to share a recent success story that might inspire you:

**Client Story:**
"[Client Name] was looking for a [property type] in [area] with a budget of $[X]. 
We found them the perfect home in just [X] weeks, and they closed [X]% below asking price!"

**What Made It Work:**
✓ Clear communication about their needs
✓ Quick response to new listings
✓ Expert negotiation skills
✓ Local market knowledge

**Results:**
- Found their dream home in [X] days
- Saved $[X] through negotiation
- Smooth closing process
- Happy client! ⭐⭐⭐⭐⭐

I'd love to create a similar success story for you!

Ready to get started? [Schedule a call] or reply to this email.

Best,
[Your Name]
```

---

### Email 5: Urgency/Scarcity (Day 12)
**Subject:** ⚠️ New Listings Won't Last Long

**Body:**
```
Hi [Name],

I wanted to give you a heads up - there are [X] new properties that just hit the market 
that match your criteria perfectly.

**Why Act Now:**
- These properties typically sell in [X] days
- Interest rates are [trending up/down]
- Spring market is heating up (or relevant seasonal trend)

**Properties to Check Out:**
1. [Property Address] - $[Price]
   - [Key features]
   - [Link to listing]

2. [Property Address] - $[Price]
   - [Key features]
   - [Link to listing]

3. [Property Address] - $[Price]
   - [Key features]
   - [Link to listing]

Want to schedule a showing? I can get you in as early as [day/time].

Reply to this email or call me at [phone number].

Best,
[Your Name]
```

---

### Email 6: Educational Content (Day 18)
**Subject:** The Home Buying Process: Step-by-Step Guide

**Body:**
```
Hi [Name],

I know the home buying process can seem overwhelming. Let me break it down for you:

**Step 1: Pre-Approval** (1-3 days)
Get your financing in order before you start looking.

**Step 2: Home Search** (2-8 weeks)
We'll tour properties that match your criteria.

**Step 3: Make an Offer** (1-2 days)
I'll help you craft a competitive offer.

**Step 4: Inspection & Negotiation** (1-2 weeks)
We'll ensure the home is in good condition.

**Step 5: Closing** (30-45 days)
Final paperwork and you get the keys!

**Timeline:** Typically 60-90 days from start to finish.

**Questions?** I'm here to guide you through every step.

Want to discuss your timeline? [Schedule a call]

Best,
[Your Name]
```

---

### Email 7: Re-engagement (Day 30)
**Subject:** Still Looking? Let's Reconnect

**Body:**
```
Hi [Name],

I noticed we haven't connected in a while. Are you still looking for your perfect home?

**I'm here to help with:**
✓ Finding properties that match your criteria
✓ Answering any questions about the process
✓ Providing market insights
✓ Negotiating the best deal

**Maybe your needs have changed?**
- Different budget range?
- Different location?
- Different timeline?
- Just browsing for now?

No pressure - just want to make sure I'm helping you in the best way possible.

Reply to this email and let me know:
1. Are you still actively looking?
2. What's your current timeline?
3. Any questions I can answer?

I'm here when you're ready!

Best,
[Your Name]
```

---

## Automation Rules

1. **Email 1**: Triggered immediately upon form submission
2. **Email 2**: Send 2 days after Email 1 (if no response)
3. **Email 3**: Send 5 days after Email 1
4. **Email 4**: Send 8 days after Email 1
5. **Email 5**: Send 12 days after Email 1
6. **Email 6**: Send 18 days after Email 1
7. **Email 7**: Send 30 days after Email 1 (if no engagement)

## Engagement Tracking

- If lead opens email → Mark as "Engaged"
- If lead clicks link → Mark as "Highly Engaged"
- If lead replies → Move to "Active Lead" sequence
- If no engagement after 30 days → Move to "Cold Lead" re-engagement

## A/B Testing Ideas

- Test different subject lines
- Test email send times (morning vs. evening)
- Test personalization levels
- Test call-to-action buttons vs. text links

---

## Integration with CRM

Connect your email platform to your CRM to:
- Track email opens and clicks
- Update lead status automatically
- Trigger follow-up tasks
- Score leads based on engagement

