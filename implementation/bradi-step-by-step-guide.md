# Bradi's Step-by-Step Implementation Guide

## Overview
This is your complete roadmap to implementing the Gippsland Property Sales marketing system. Follow this day-by-day to get everything set up and generating appraisals.

**Estimated Time**: 2-3 weeks (working part-time) or 1 week (full-time focus)

---

## Pre-Implementation Checklist

Before you start, gather this information:
- [ ] Business phone number (Australian format)
- [ ] Business email address
- [ ] Office address (for Google Business Profile)
- [ ] Team member names and roles
- [ ] Current property listings (for content)
- [ ] Recent client testimonials
- [ ] Professional photos (team, properties, office)

---

## WEEK 1: Foundation & Setup

### Day 1: Company Information & Planning (2-3 hours)

**Morning (1.5 hours):**
1. **Review Company Info File**
   - Open `/company-info/gippsland-property-sales-info.md`
   - Fill in any missing details (phone, email, addresses)
   - Verify all team member names

2. **Review Funnel Flow**
   - Read `/funnels/appraisal-funnel-flow.md`
   - Understand the complete process
   - Note any questions

**Afternoon (1 hour):**
3. **Plan Your Timeline**
   - Decide when you want to launch (coordinate with rebrand if needed)
   - Block out time in calendar for implementation
   - Set up project management (if using)

4. **Choose Your Tools**
   - Email platform: Mailchimp (free) or ConvertKit (free) or HubSpot (free)
   - CRM: Google Sheets (free) or HubSpot (free)
   - Form handler: EmailJS (free) or Formspree (free)
   - Decide now so you're ready for Day 2

---

### Day 2: Landing Pages Setup (3-4 hours)

**Morning (2 hours):**
1. **Review Landing Pages**
   - Open `/landing-pages/appraisal-landing-page.html`
   - Open `/landing-pages/home-buyers-landing.html`
   - Review the code and structure

2. **Customise Landing Pages**
   - Replace any placeholder text with your actual information
   - Add your phone number (Australian format)
   - Add your email address
   - Verify all Gippsland locations are correct

**Afternoon (2 hours):**
3. **Set Up Form Submission**
   - Choose form handler (EmailJS recommended - free)
   - Sign up for EmailJS at [emailjs.com](https://www.emailjs.com)
   - Create email template in EmailJS
   - Get your EmailJS service ID, template ID, and public key
   - Add EmailJS code to landing pages
   - Test form submission

4. **Host Landing Pages**
   - **Option 1: Netlify (Recommended - Free)**
     - Sign up at [netlify.com](https://www.netlify.com)
     - Drag and drop your HTML files
     - Get free URL (e.g., `gippsland-appraisals.netlify.app`)
     - Option to add custom domain later
   - **Option 2: Your Own Hosting**
     - Upload HTML files to your web host
     - Create subdomain (e.g., `appraisals.yourdomain.com.au`)
   - **Option 3: GitHub Pages (Free)**
     - Upload to GitHub repository
     - Enable GitHub Pages
     - Get free URL

**Test:**
- [ ] Submit test form
- [ ] Verify email is received
- [ ] Check form on mobile device
- [ ] Test all links work

---

### Day 3: Email Automation Setup (3-4 hours)

**Morning (2 hours):**
1. **Choose Email Platform**
   - Sign up for Mailchimp (free up to 500 contacts) OR
   - Sign up for ConvertKit (free up to 1,000 subscribers) OR
   - Sign up for HubSpot (free up to 1,000 contacts)
   - **Recommendation**: Start with Mailchimp (easiest)

2. **Import Email Templates**
   - Open `/email-automation/gippsland-email-templates.md`
   - Copy email templates into your email platform
   - Customise with your name, phone, email
   - Replace [Name], [Suburb] with merge tags

**Afternoon (2 hours):**
3. **Set Up Automation Sequence**
   - Create automation workflow
   - Set up 7-email sequence:
     - Email 1: Immediate (triggered by form submission)
     - Email 2: 2 days delay
     - Email 3: 5 days delay
     - Email 4: 8 days delay
     - Email 5: 12 days delay
     - Email 6: 18 days delay
     - Email 7: 30 days delay
   - Set up conditions (pause if lead responds)

4. **Connect Email to Landing Page**
   - Update landing page form to add subscribers to email list
   - Test: Submit form → Check email automation triggers
   - Verify welcome email is sent

**Test:**
- [ ] Submit test form
- [ ] Verify welcome email received
- [ ] Check email automation is set up correctly

---

### Day 4: CRM Setup (2-3 hours)

**Morning (1.5 hours):**
1. **Set Up CRM**
   - **Option 1: Google Sheets (Recommended - Free)**
     - Create new Google Sheet
     - Name it "Gippsland Property Sales Leads 2025"
     - Create columns: Date, Name, Email, Phone, Address, Suburb, Timeline, Property Type, Source, Status, Assigned To, Notes, Follow-up Date
     - Set up data validation for Status column (dropdown)
     - Set up conditional formatting (highlight new leads)
   - **Option 2: HubSpot (Free)**
     - Create custom properties
     - Set up deal pipeline
     - Create email templates

2. **Connect Form to CRM**
   - Set up Zapier (free tier) to connect form → CRM OR
   - Use Google Forms and connect to Google Sheets OR
   - Manually copy leads (not recommended, but works)

**Afternoon (1 hour):**
3. **Set Up Follow-Up Process**
   - Create email template for Mel & Jeff
   - Set up calendar reminders (if using Google Calendar)
   - Create task management system (if needed)

**Test:**
- [ ] Submit test form
- [ ] Verify lead appears in CRM
- [ ] Test follow-up notification

---

### Day 5: Tracking & Analytics Setup (2-3 hours)

**Morning (1.5 hours):**
1. **Set Up Google Analytics 4**
   - Create GA4 account at [analytics.google.com](https://analytics.google.com)
   - Get your Measurement ID (G-XXXXXXXXXX)
   - Add tracking code to landing pages
   - Set up conversion events:
     - Form submission
     - Phone call clicks
     - Email clicks

2. **Set Up Google Search Console**
   - Add property at [search.google.com/search-console](https://search.google.com/search-console)
   - Verify ownership
   - Submit sitemap (if you have one)

**Afternoon (1.5 hours):**
3. **Set Up Facebook Pixel**
   - Go to Facebook Events Manager
   - Create Pixel
   - Get Pixel ID
   - Add Pixel code to landing pages
   - Test Pixel is working (use Facebook Pixel Helper browser extension)

4. **Set Up Tracking Dashboard**
   - Create Google Sheet for tracking metrics
   - Set up columns: Date, Source, Clicks, Leads, Cost, Cost per Lead, Appraisals, Listings
   - Create formulas to calculate metrics automatically

**Test:**
- [ ] Visit landing page
- [ ] Check Google Analytics shows visit
- [ ] Check Facebook Pixel fires
- [ ] Submit test form and verify conversion tracking

---

## WEEK 2: Content & Pre-Launch

### Day 6: Google Business Profile Optimisation (2-3 hours)

**Morning (1.5 hours):**
1. **Claim/Optimise Google Business Profile**
   - Go to [google.com/business](https://www.google.com/business)
   - Claim or create your business profile
   - Complete ALL sections:
     - Business name: @realty Property Sales Gippsland
     - Address: Your Gippsland office address
     - Phone: Australian format
     - Category: Real Estate Agency
     - Service areas: Drouin, Trafalgar, Warragul, Moe, Traralgon, Gippsland
     - Hours: Your business hours
     - Description: Include keywords (real estate agent Gippsland, property sales Drouin, etc.)

2. **Add Photos**
   - Upload 20+ high-quality photos
   - Include: Office exterior, team photos, property photos, local area photos
   - Add logo as profile photo

**Afternoon (1.5 hours):**
3. **Set Up Google Posts**
   - Create first post (welcome post or current listing)
   - Plan content calendar (2-3 posts per week)
   - Set up Q&A section (add common questions)

4. **Request Reviews**
   - Identify past clients to ask for reviews
   - Send review request emails with direct link
   - Follow up if needed

---

### Day 7: Australian Platform Profiles (3-4 hours)

**Morning (2 hours):**
1. **RealEstate.com.au Profile**
   - Go to [realestate.com.au/agent](https://www.realestate.com.au/agent)
   - Create or claim your agent profile
   - Complete profile:
     - Professional photo
     - Bio highlighting Gippsland expertise
     - Service areas: Drouin, Trafalgar, Warragul, etc.
     - Contact information
     - Specialisations
   - Link to your listings

2. **Domain.com.au Profile**
   - Go to [domain.com.au](https://www.domain.com.au)
   - Create or claim your agent profile
   - Similar optimisation to RealEstate.com.au

**Afternoon (2 hours):**
3. **Other Australian Citations**
   - TrueLocal (truelocal.com.au)
   - Yellow Pages Australia (yellowpages.com.au)
   - LocalSearch (localsearch.com.au)
   - Bing Places for Business

4. **Social Media Setup**
   - Ensure Facebook Business Page is optimised
   - Ensure Instagram profile is set up
   - Add links to landing pages in bio/description

---

### Day 8: Ad Account Setup (2-3 hours)

**Morning (1.5 hours):**
1. **Google Ads Account**
   - Create account at [ads.google.com](https://ads.google.com)
   - Set currency to AUD
   - Set location to Gippsland, Victoria, Australia
   - Set up billing (don't add payment yet if not ready to launch)
   - Create first campaign structure (don't launch yet)

2. **Review Ad Templates**
   - Open `/ad-templates/google-ads-australia.md`
   - Review campaign structure
   - Note which campaigns you'll start with (recommend: Property Appraisals first)

**Afternoon (1.5 hours):**
3. **Facebook Business Manager**
   - Create Business Manager account
   - Create Facebook Page (if you don't have one)
   - Set up Facebook Pixel (already done on Day 5, but verify)

4. **Review Facebook Ad Templates**
   - Open `/ad-templates/facebook-ads-australia.md`
   - Review campaign structure
   - Note which ad sets you'll start with

---

### Day 9: Content Creation (3-4 hours)

**Morning (2 hours):**
1. **Create First Blog Post**
   - Topic: "Ultimate Guide to Buying a Home in Gippsland 2025"
   - 1,500+ words
   - Include: Drouin, Trafalgar, Warragul market data
   - Optimise for SEO (use keywords from SEO guide)
   - Publish on your website (if you have blog) OR
   - Publish on Medium/LinkedIn (if no website blog yet)

2. **Create Social Media Content**
   - Plan 2 weeks of social media posts
   - Mix of: Property listings, market updates, tips, local area highlights
   - Use Canva (free) to create graphics

**Afternoon (2 hours):**
3. **Prepare Ad Creative**
   - Take/collect property photos
   - Create ad images (use Canva)
   - Write ad copy variations
   - Prepare video scripts (if doing video ads)

---

### Day 10: Final Testing & Preparation (3-4 hours)

**Morning (2 hours):**
1. **Complete Testing**
   - Test landing page on multiple devices (desktop, tablet, mobile)
   - Test form submission end-to-end
   - Verify email automation works
   - Check CRM entries
   - Verify tracking (Google Analytics, Facebook Pixel)
   - Test on different browsers

2. **Create Pre-Launch Checklist**
   - Use `/implementation/pre-launch-checklist.md`
   - Go through every item
   - Fix any issues

**Afternoon (2 hours):**
3. **Prepare Launch Materials**
   - Finalise ad copy
   - Prepare ad creative
   - Set up ad campaigns (don't launch yet)
   - Prepare budget allocation
   - Create monitoring schedule

4. **Team Briefing**
   - Brief Mel & Jeff on follow-up process
   - Explain CRM system
   - Set expectations for response times
   - Create follow-up scripts

---

## WEEK 3: Launch & Optimisation

### Day 11: Soft Launch (2-3 hours)

**Morning (1 hour):**
1. **Launch Google Ads (Small Budget)**
   - Start with Property Appraisals campaign only
   - Budget: $20-30 AUD/day
   - Launch campaign
   - Monitor closely

**Afternoon (1-2 hours):**
2. **Launch Facebook Ads (Small Budget)**
   - Start with Property Appraisals ad set only
   - Budget: $10-15 AUD/day
   - Launch campaign
   - Monitor closely

3. **Set Up Monitoring**
   - Check ads are showing
   - Monitor landing page traffic
   - Watch for form submissions
   - Set up daily check-in routine

---

### Day 12-14: Monitor & Optimise (1-2 hours/day)

**Daily Tasks:**
- [ ] Check Google Ads performance
- [ ] Check Facebook Ads performance
- [ ] Review landing page analytics
- [ ] Check for new leads in CRM
- [ ] Verify Mel/Jeff are following up
- [ ] Review search terms (add negative keywords)
- [ ] Check ad spend vs. budget
- [ ] Monitor cost per lead

**Optimisation:**
- Pause underperforming keywords/ads
- Increase bids on winners
- Add negative keywords
- Test new ad copy
- Adjust targeting if needed

---

### Day 15: First Week Review (2-3 hours)

**Review:**
- Total ad spend
- Number of clicks
- Number of leads
- Cost per lead
- Number of appraisals scheduled
- What's working
- What's not working

**Adjustments:**
- Scale winning campaigns
- Pause or fix underperformers
- Adjust budgets
- Plan next week's strategy

---

## Ongoing Weekly Routine

### Monday Morning (30 min):
- Review last week's metrics
- Check Google Ads performance
- Check Facebook Ads performance
- Review new leads in CRM
- Plan follow-ups for the week

### Daily (10 min):
- Check for new leads
- Respond to leads within 1 hour (or assign to Mel/Jeff)
- Monitor ad performance
- Post on Google Business Profile (2-3x per week)

### Friday Afternoon (30 min):
- Review week's performance
- Update metrics dashboard
- Plan next week's content
- Schedule social media posts

---

## Monthly Routine

### First Monday of Month (2 hours):
- Review last month's performance
- Calculate ROI
- Identify what worked
- Identify what to improve
- Plan next month's strategy
- Update budget if needed

---

## Troubleshooting Guide

### "I'm not getting any leads"
- Check: Are your ads running? (Check ad status in Google Ads/Facebook Ads)
- Check: Are your landing pages working? (Test form)
- Check: Is your targeting too narrow? (Expand audience)
- Check: Are your ads showing? (Check impressions)
- Check: Are your keywords too competitive? (Try long-tail keywords)

### "Leads are too expensive"
- Improve landing page (better conversion rate = lower cost per lead)
- Refine targeting (more specific = better quality)
- Test new ad copy (better CTR = lower CPC)
- Optimise keywords (remove low-performing)
- Improve ad relevance score

### "Leads aren't converting to appraisals"
- Follow up faster (within 1 hour for hot leads)
- Improve qualification process
- Nurture leads longer (email sequence)
- Improve follow-up scripts
- Train Mel/Jeff on conversion techniques

### "Appraisals aren't converting to listings"
- This is Mel & Jeff's expertise area
- Improve appraisal presentation
- Better market analysis
- Stronger listing proposal
- Follow-up process

---

## Key Resources

**Files to Reference:**
- `/funnels/appraisal-funnel-flow.md` - Complete funnel process
- `/ad-templates/google-ads-australia.md` - Google Ads templates
- `/ad-templates/facebook-ads-australia.md` - Facebook Ads templates
- `/email-automation/gippsland-email-templates.md` - Email templates
- `/seo/australian-seo-guide.md` - SEO guide
- `/integration/franchise-website-workaround.md` - Landing page hosting solutions

**External Resources:**
- Google Ads Help: [support.google.com/google-ads](https://support.google.com/google-ads)
- Facebook Ads Help: [facebook.com/business/help](https://www.facebook.com/business/help)
- Mailchimp Help: [mailchimp.com/help](https://mailchimp.com/help)

---

## Budget Recommendations

### Starting Budget (Month 1):
- **Google Ads**: $500-1,000 AUD/month ($20-35/day)
- **Facebook Ads**: $300-500 AUD/month ($10-15/day)
- **Tools**: $0-50 AUD/month (optional email service upgrade)
- **Total**: $800-1,550 AUD/month

### Scaling Budget (Month 3+):
- **Google Ads**: $1,000-2,000 AUD/month (if performing well)
- **Facebook Ads**: $500-1,000 AUD/month (if performing well)
- **Tools**: $50-100 AUD/month
- **Total**: $1,550-3,100 AUD/month

**Remember**: Only scale what's working! If Google Ads performs better, put more budget there.

---

## Success Metrics

### Primary Goal: Appraisals
- Track: Appraisal requests per month
- Target: 20-50 appraisals/month (from online leads)
- Conversion: Appraisals → Listings (Mel & Jeff's expertise)

### Key Metrics:
- Cost per lead (target: $40-150 AUD)
- Cost per appraisal (target: $50-150 AUD)
- Appraisal → Listing conversion rate (target: 30-50%)
- ROI: (Commission from listings - Ad spend) / Ad spend

---

## Next Steps After Implementation

1. **Week 4+**: Continue monitoring and optimising
2. **Month 2**: Scale winning campaigns
3. **Month 3**: Add new campaigns (home buyers, suburb-specific)
4. **Ongoing**: Content creation, SEO, local marketing

---

## Questions?

If you get stuck:
1. Check the specific guide for that topic
2. Google the specific issue (all tools have great documentation)
3. Start simple, then add complexity as you learn

**Remember**: You're building a marketing system that will work for years to come. Take it one step at a time, and don't try to do everything at once!

---

*This guide is your complete roadmap. Follow it step-by-step, and you'll have a fully functional marketing system generating appraisals in 2-3 weeks.*

