# Franchise Website Workaround Solutions

## Overview
Since your main website (atrealtypropertysalesgippsland.com.au) is managed by @realty head office, you need standalone landing pages for full control over your marketing campaigns. This guide provides complete solutions.

---

## Why Standalone Landing Pages Are Better

**Even if you had full website control, standalone landing pages are best practice because:**
- ✅ Focused on conversion (no navigation distractions)
- ✅ Easy to A/B test
- ✅ Fast loading (no heavy website code)
- ✅ Complete control over design and tracking
- ✅ Can update instantly without head office approval
- ✅ Standard practice in digital marketing

**King Kong would do the same thing** - they'd create separate landing pages even if you had website access.

---

## Solution Options (Ranked by Recommendation)

### Option 1: Netlify (RECOMMENDED - Free & Easy)

**Best For:** Quick setup, no technical knowledge needed

**Setup:**
1. Sign up at [netlify.com](https://www.netlify.com) (free)
2. Drag and drop your HTML files
3. Get instant free URL: `your-name.netlify.app`
4. Option to add custom domain later (e.g., `appraisals.gippslandproperty.com.au`)

**Pros:**
- ✅ Completely free
- ✅ No technical knowledge needed
- ✅ Instant setup (5 minutes)
- ✅ Automatic HTTPS (secure)
- ✅ Fast loading
- ✅ Can add custom domain later

**Cons:**
- Free URL includes "netlify.app" (but you can add custom domain)

**Cost:** Free (or $19/month for custom domain + features)

---

### Option 2: Your Own Hosting

**Best For:** Full control, branded URLs

**Setup:**
1. Buy domain: `gippslandpropertyappraisals.com.au` (~$15-30 AUD/year)
2. Get web hosting (~$5-15 AUD/month)
3. Upload HTML files via FTP
4. Point domain to hosting

**Pros:**
- ✅ Complete control
- ✅ Branded URL
- ✅ Professional appearance
- ✅ Can add more pages later

**Cons:**
- Requires hosting account
- Slightly more technical
- Ongoing hosting costs

**Cost:** ~$15-30 AUD/year (domain) + $5-15 AUD/month (hosting)

**Recommended Hosts:**
- SiteGround (Australian-friendly)
- Hostinger (cheap)
- Bluehost (popular)

---

### Option 3: GitHub Pages (Free)

**Best For:** Developers, version control

**Setup:**
1. Create GitHub account (free)
2. Create repository
3. Upload HTML files
4. Enable GitHub Pages
5. Get free URL: `yourusername.github.io/your-site`

**Pros:**
- ✅ Completely free
- ✅ Version control
- ✅ Can add custom domain

**Cons:**
- More technical
- Requires GitHub knowledge
- URL includes "github.io" (unless custom domain)

**Cost:** Free

---

### Option 4: Vercel (Free)

**Best For:** Modern developers, fast performance

**Setup:**
1. Sign up at [vercel.com](https://www.vercel.com) (free)
2. Connect GitHub or upload files
3. Get instant free URL
4. Option to add custom domain

**Pros:**
- ✅ Completely free
- ✅ Very fast
- ✅ Easy setup
- ✅ Automatic HTTPS

**Cons:**
- Free URL includes "vercel.app" (unless custom domain)

**Cost:** Free

---

## Recommended Setup: Netlify (Step-by-Step)

### Step 1: Sign Up
1. Go to [netlify.com](https://www.netlify.com)
2. Click "Sign up" (use email or GitHub)
3. Verify your email

### Step 2: Upload Landing Pages
1. In Netlify dashboard, click "Add new site"
2. Choose "Deploy manually"
3. Drag and drop your HTML files:
   - `appraisal-landing-page.html`
   - `home-buyers-landing.html`
   - Any other HTML files
4. Click "Deploy site"
5. Wait 30 seconds - your site is live!

### Step 3: Get Your URL
- Netlify gives you a URL like: `random-name-12345.netlify.app`
- You can rename it: Go to Site settings → Change site name
- Example: `gippsland-appraisals.netlify.app`

### Step 4: Test Your Site
- Visit your URL
- Test the form submission
- Check on mobile device
- Verify everything works

### Step 5: (Optional) Add Custom Domain
- Go to Site settings → Domain management
- Add custom domain (e.g., `appraisals.gippslandproperty.com.au`)
- Follow DNS instructions
- Wait for DNS propagation (24-48 hours)

---

## Form Integration Options

Since you can't modify the main website, use external form services:

### Option 1: EmailJS (RECOMMENDED - Free)

**Setup:**
1. Sign up at [emailjs.com](https://www.emailjs.com) (free)
2. Create email service (Gmail, Outlook, etc.)
3. Create email template
4. Get Service ID, Template ID, and Public Key
5. Add EmailJS code to your landing page

**Code to Add:**
```html
<!-- Add to <head> -->
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
<script>
  (function(){
    emailjs.init("YOUR_PUBLIC_KEY");
  })();
</script>

<!-- Update form submission -->
<script>
function handleSubmit(event) {
  event.preventDefault();
  
  emailjs.sendForm('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', event.target)
    .then(function() {
      alert('Thank you! We\'ll contact you shortly.');
      event.target.reset();
    }, function(error) {
      alert('Sorry, there was an error. Please try again.');
    });
}
</script>
```

**Pros:**
- ✅ Free (200 emails/month)
- ✅ Easy setup
- ✅ Sends directly to your email
- ✅ No backend needed

**Cost:** Free (or $15/month for 1,000 emails)

---

### Option 2: Formspree (Free)

**Setup:**
1. Sign up at [formspree.io](https://formspree.io) (free)
2. Get your form endpoint URL
3. Update form action to Formspree URL

**Code:**
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
  <!-- Your form fields -->
</form>
```

**Pros:**
- ✅ Free (50 submissions/month)
- ✅ Very easy
- ✅ Spam protection

**Cost:** Free (or $10/month for 1,000 submissions)

---

### Option 3: Google Forms (Free)

**Setup:**
1. Create Google Form matching your landing page fields
2. Get embed code
3. Replace form on landing page with Google Form embed
4. Responses go to Google Sheet automatically

**Pros:**
- ✅ Completely free
- ✅ Unlimited submissions
- ✅ Automatic spreadsheet
- ✅ Easy to share

**Cons:**
- Less customisable design
- Google branding (unless you style it)

**Cost:** Free

---

### Option 4: HubSpot Forms (Free CRM)

**Setup:**
1. Sign up for HubSpot (free)
2. Create form in HubSpot
3. Get embed code
4. Add to landing page

**Pros:**
- ✅ Free CRM included
- ✅ Automatic lead entry
- ✅ Email automation integration
- ✅ Professional forms

**Cost:** Free (up to 1,000 contacts)

---

## Connecting to Main Website

### Option 1: Redirect from Main Site

**If head office allows:**
- Update "Book Appraisal" button on main site
- Link to your standalone landing page
- Example: `https://appraisals.gippslandproperty.com.au`

**Benefits:**
- Maintains brand consistency
- Uses existing traffic
- Professional appearance

---

### Option 2: Subdomain Request

**Request from head office:**
- Ask for subdomain: `appraisals.atrealtypropertysalesgippsland.com.au`
- You control the subdomain
- Host your landing pages there

**Benefits:**
- Branded URL
- Maintains @realty branding
- Full control over subdomain

---

### Option 3: Separate Domain

**Buy your own domain:**
- `gippslandpropertyappraisals.com.au`
- `gippslandappraisals.com.au`
- Host landing pages there

**Benefits:**
- Complete independence
- Full control
- Can use for other marketing

**Cost:** ~$15-30 AUD/year

---

## Tracking Setup (Standalone Pages)

### Google Analytics
Add to `<head>`:
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

### Facebook Pixel
Add to `<head>`:
```html
<!-- Facebook Pixel Code -->
<script>
!function(f,b,e,v,n,t,s)
{if(f.fbq)return;n=f.fbq=function(){n.callMethod?
n.callMethod.apply(n,arguments):n.queue.push(arguments)};
if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
n.queue=[];t=b.createElement(e);t.async=!0;
t.src=v;s=b.getElementsByTagName(e)[0];
s.parentNode.insertBefore(t,s)}(window, document,'script',
'https://connect.facebook.net/en_US/fbevents.js');
fbq('init', 'YOUR_PIXEL_ID');
fbq('track', 'PageView');
</script>
```

### Google Ads Conversion Tracking
Add to thank you page or form submission handler:
```html
<script>
gtag('event', 'conversion', {
  'send_to': 'AW-XXXXXXXXXX/XXXXXXXXXX',
  'value': 1.0,
  'currency': 'AUD'
});
</script>
```

---

## Recommended Complete Setup

**For Gippsland Property Sales, I recommend:**

1. **Hosting**: Netlify (free, easy, fast)
2. **Form Handler**: EmailJS (free, sends to your email)
3. **CRM**: Google Sheets (free, simple)
4. **Email Automation**: Mailchimp (free up to 500 contacts)
5. **Domain**: Request subdomain from head office OR use Netlify free URL initially

**Total Setup Cost: $0 AUD/month**

---

## Testing Checklist

Before going live:
- [ ] Landing page loads quickly (< 3 seconds)
- [ ] Form submits successfully
- [ ] Email is received when form is submitted
- [ ] Landing page works on mobile
- [ ] Landing page works on tablet
- [ ] All links work
- [ ] Tracking codes are firing (Google Analytics, Facebook Pixel)
- [ ] Conversion tracking works
- [ ] Thank you message displays

---

## Maintenance

**Weekly:**
- Check landing page is still live
- Test form submission
- Review analytics

**Monthly:**
- Update content if needed
- A/B test new headlines
- Optimise based on data

---

## FAQ

**Q: Do I need head office approval?**
A: No, if you host separately. But it's good to inform them.

**Q: Can I use @realty branding?**
A: Check your franchise agreement. Usually yes for marketing materials.

**Q: What if head office wants to integrate later?**
A: You can always redirect or move pages. Your standalone pages work independently.

**Q: Will this work with the rebrand?**
A: Yes! You can update landing pages instantly when rebrand is complete.

---

## Next Steps

1. Choose hosting option (Netlify recommended)
2. Set up form handler (EmailJS recommended)
3. Upload landing pages
4. Test everything
5. Launch!

---

*This solution gives you complete control over your marketing while working within the franchise structure. You can launch immediately without waiting for head office approval.*

