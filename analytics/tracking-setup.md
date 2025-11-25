# Analytics & Tracking Setup Guide

## Overview
Track everything: website visitors, form submissions, ad performance, phone calls, and revenue. This is how you'll know what's working and what's not.

---

## Essential Tracking Tools (All FREE)

### 1. Google Analytics 4 (GA4)
**What it tracks:** Website visitors, page views, user behavior, conversions

### 2. Google Search Console
**What it tracks:** SEO performance, search rankings, keyword performance

### 3. Google Business Profile Insights
**What it tracks:** How people find your business, search queries, actions taken

### 4. Google Ads Dashboard
**What it tracks:** Ad performance, clicks, conversions, cost per lead

### 5. Facebook Ads Manager
**What it tracks:** Facebook ad performance, reach, engagement, conversions

---

## 1. Google Analytics 4 Setup

### Step 1: Create GA4 Property
1. Go to [analytics.google.com](https://analytics.google.com)
2. Create account (if you don't have one)
3. Create new property
4. Name it: "[Your Business] Website"

### Step 2: Install Tracking Code

Add this to your website's `<head>` section (on every page):

```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

Replace `G-XXXXXXXXXX` with your actual Measurement ID from GA4.

### Step 3: Set Up Conversions

**Conversion Event 1: Form Submission**

Add this to your form submission handler:
```javascript
// When form is successfully submitted
gtag('event', 'form_submission', {
  'form_name': 'lead_form',
  'form_location': 'landing_page'
});
```

**Conversion Event 2: Phone Call Click**

Add this to your phone number links:
```html
<a href="tel:+1234567890" onclick="gtag('event', 'phone_call', {'event_category': 'contact', 'event_label': 'header_phone'});">Call Us</a>
```

**Conversion Event 3: Email Click**

Add this to your email links:
```html
<a href="mailto:you@email.com" onclick="gtag('event', 'email_click', {'event_category': 'contact'});">Email Us</a>
```

### Step 4: Set Up Goals in GA4

1. Go to Admin → Events
2. Mark these as "Conversions":
   - `form_submission`
   - `phone_call`
   - `email_click`

### Key Metrics to Track:
- **Users**: Total website visitors
- **Sessions**: Total visits
- **Bounce Rate**: % who leave immediately (aim for <50%)
- **Average Session Duration**: Time on site (aim for >2 minutes)
- **Conversions**: Form submissions, calls, emails
- **Conversion Rate**: Conversions / Sessions (aim for 2-5%)

---

## 2. Google Search Console Setup

### Step 1: Add Property
1. Go to [search.google.com/search-console](https://search.google.com/search-console)
2. Add property (your website URL)
3. Verify ownership (HTML tag method is easiest)

### Step 2: Submit Sitemap
1. Create sitemap.xml (or use online generator)
2. Submit to Search Console
3. Helps Google index your pages faster

### Key Metrics to Track:
- **Impressions**: How many times you appeared in search
- **Clicks**: How many people clicked to your site
- **Average Position**: Your ranking (aim for top 10)
- **Click-Through Rate (CTR)**: Clicks / Impressions (aim for 3-5%)
- **Top Queries**: What people search to find you
- **Top Pages**: Your most popular pages

---

## 3. Google Business Profile Insights

### Access:
1. Go to [google.com/business](https://www.google.com/business)
2. Select your business
3. Click "Insights" in left menu

### Key Metrics:
- **How customers find you**: Search vs. Maps
- **Search queries**: What people search to find you
- **Customer actions**: Website visits, direction requests, calls
- **Photo views**: How many people view your photos
- **Post engagement**: How many people engage with your posts

---

## 4. Google Ads Tracking

### Conversion Tracking Setup:

**Step 1: Create Conversion Action**
1. Go to Google Ads → Tools → Conversions
2. Click "+" to create new conversion
3. Choose "Website"
4. Name it: "Lead Form Submission"
5. Copy the conversion tag code

**Step 2: Install Conversion Tag**

Add to your thank you page (after form submission):
```html
<!-- Google Ads Conversion Tag -->
<script async src="https://www.googletagmanager.com/gtag/js?id=AW-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'AW-XXXXXXXXXX');
</script>

<!-- Conversion Event -->
<script>
  gtag('event', 'conversion', {
    'send_to': 'AW-XXXXXXXXXX/XXXXXXXXXX',
    'value': 1.0,
    'currency': 'USD'
  });
</script>
```

### Key Metrics to Track:
- **Impressions**: How many times your ad was shown
- **Clicks**: How many people clicked
- **CTR**: Click-through rate (aim for 3-7%)
- **Cost per Click (CPC)**: Average cost per click
- **Conversions**: Form submissions/calls from ads
- **Cost per Conversion**: Ad spend / conversions (aim for <$150)
- **ROAS**: Return on ad spend (revenue / ad spend)

---

## 5. Facebook Pixel Tracking

### Setup:
1. Go to Facebook Events Manager
2. Create Pixel
3. Copy pixel code
4. Add to website `<head>`

### Track Conversions:

**Form Submission:**
```javascript
fbq('track', 'Lead');
```

**Property View:**
```javascript
fbq('track', 'ViewContent', {
  content_name: 'Property Listing',
  content_category: 'Real Estate'
});
```

### Key Metrics:
- **Reach**: How many people saw your ad
- **Impressions**: Total ad views
- **Clicks**: People who clicked
- **CTR**: Click-through rate (aim for 1-3%)
- **Cost per Click**: Average CPC (aim for $0.50-2.00)
- **Cost per Lead**: Ad spend / leads (aim for $10-50)
- **ROAS**: Return on ad spend

---

## 6. Call Tracking (Advanced)

### Option 1: Google Call Tracking
- Use Google Ads call extensions
- Track calls directly in Google Ads
- Free with Google Ads

### Option 2: CallRail (Paid, but worth it)
- $45/month
- Track calls from all sources
- Record calls
- See which ads generate calls

### Option 3: Simple Method
- Ask every caller: "How did you hear about us?"
- Track in your CRM/spreadsheet
- Free but requires discipline

---

## 7. Revenue Tracking

### Track in Your CRM/Spreadsheet:

**Monthly Metrics:**
- Total leads generated
- Leads by source (Google Ads, Facebook, SEO, etc.)
- Total closed deals
- Revenue generated
- Cost per lead (ad spend / leads)
- Cost per closed deal (ad spend / closed deals)
- ROI: (Revenue - Total Marketing Cost) / Total Marketing Cost

### Example Calculation:
```
Monthly Ad Spend: $1,000
Leads Generated: 20
Cost per Lead: $50
Closed Deals: 2
Average Commission: $5,000
Total Revenue: $10,000
ROI: ($10,000 - $1,000) / $1,000 = 900%
```

---

## Dashboard Setup

### Create a Simple Dashboard (Google Sheets):

**Weekly Metrics Sheet:**
```
Week | Leads | Google Ads Leads | Facebook Leads | SEO Leads | Calls | Forms | Closed Deals | Revenue
-----|-------|-----------------|----------------|-----------|-------|-------|--------------|--------
1/1  | 15    | 8               | 5              | 2         | 10    | 5     | 1            | $5,000
1/8  | 18    | 10              | 6              | 2         | 12    | 6     | 2            | $10,000
```

**Monthly Summary:**
```
Metric                    | Value
--------------------------|--------
Total Leads               | 65
Google Ads Leads          | 35
Facebook Leads            | 20
SEO Leads                 | 10
Total Ad Spend            | $2,000
Cost per Lead             | $30.77
Closed Deals              | 5
Close Rate                | 7.7%
Total Revenue             | $25,000
ROI                       | 1,150%
```

---

## Weekly Review Checklist

Every Monday, review:

- [ ] Google Analytics: Website traffic, conversions
- [ ] Google Search Console: Search rankings, clicks
- [ ] Google Business Profile: Actions, search queries
- [ ] Google Ads: Performance, cost per lead
- [ ] Facebook Ads: Performance, cost per lead
- [ ] CRM: New leads, follow-ups needed
- [ ] Revenue: Closed deals, ROI

---

## Monthly Review

At end of each month:

1. **Traffic Sources:**
   - Which source brings most traffic?
   - Which source has best conversion rate?
   - Which source generates most revenue?

2. **Content Performance:**
   - Which blog posts get most traffic?
   - Which landing pages convert best?
   - What content should you create more of?

3. **Ad Performance:**
   - Which ads perform best?
   - Which keywords convert?
   - What's your ROI?

4. **Optimization Opportunities:**
   - What's working? (do more)
   - What's not working? (fix or pause)
   - What should you test next?

---

## Cost Comparison

| Service | King Kong | DIY |
|---------|-----------|-----|
| Analytics Setup | Included | $0 |
| Tracking Implementation | Included | $0 |
| Reporting Dashboard | Included | $0 |
| Monthly Analysis | Included | $0 (your time) |
| **Total** | **$18,000** | **$0** |

---

## Quick Start Checklist

- [ ] Set up Google Analytics 4
- [ ] Install GA4 tracking code on website
- [ ] Set up conversion events
- [ ] Set up Google Search Console
- [ ] Submit sitemap
- [ ] Set up Google Business Profile
- [ ] Set up Google Ads conversion tracking
- [ ] Set up Facebook Pixel
- [ ] Create tracking dashboard (Google Sheets)
- [ ] Set up weekly review process

---

## Pro Tips

1. **Start Simple**: Don't try to track everything at once
2. **Focus on Conversions**: Traffic is nice, but conversions pay bills
3. **Review Weekly**: Don't wait until end of month
4. **Test Everything**: Always be testing and optimizing
5. **Track Revenue**: Don't just track leads, track closed deals and ROI

---

## Need Help?

All these tools are free and have excellent documentation. Start with Google Analytics and Google Business Profile - those are the most important for real estate.

Remember: What gets measured gets improved!

