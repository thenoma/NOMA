# 🌐 Custom Domain Setup for NOMA Website

## 📋 Overview

Your website is currently live at: `https://thenoma.github.io/NOMA/`

This guide will help you set up a custom domain like `nomausa.org` or `noma-usa.org`

---

## 💰 Cost

- **Domain Name**: $10-20 per year (varies by registrar and extension)
- **GitHub Pages Hosting**: FREE (forever)
- **SSL Certificate**: FREE (provided by GitHub)

**Total Annual Cost**: Just the domain registration fee!

---

## 🛒 Step 1: Buy Your Domain

### Recommended Domain Registrars:

#### **Option A: Namecheap** (Most Popular - Best Value)
- Website: https://www.namecheap.com
- Cost: ~$10-15/year for .org
- Pros: Great prices, easy DNS management, good support
- **Recommended for beginners**

#### **Option B: Google Domains / Squarespace Domains**
- Website: https://domains.squarespace.com
- Cost: ~$12-20/year
- Pros: Clean interface, integrated with Google services
- Note: Google Domains was acquired by Squarespace in 2023

#### **Option C: Cloudflare Registrar**
- Website: https://www.cloudflare.com/products/registrar/
- Cost: ~$9-12/year (at-cost pricing, no markup)
- Pros: Lowest prices, includes free CDN and security features
- Cons: Need to transfer domain (can't register initially here for some TLDs)

#### **Option D: Porkbun**
- Website: https://porkbun.com
- Cost: ~$8-11/year
- Pros: Very cheap, includes free WHOIS privacy
- Good alternative to Namecheap

### Domain Name Suggestions:
- `nomausa.org` (BEST - professional, clear)
- `noma-usa.org`
- `moroccansinamerica.org`
- `thenoma.org`
- `nomausa.com` (if .org is taken)

---

## ⚙️ Step 2: Configure DNS Settings

After purchasing your domain, you need to point it to GitHub Pages.

### DNS Configuration (Choose A or B):

#### **A. For Apex Domain** (e.g., `nomausa.org`)

Add these **4 A records** pointing to GitHub's servers:

| Type | Host | Value | TTL |
|------|------|-------|-----|
| A | @ | 185.199.108.153 | 3600 |
| A | @ | 185.199.109.153 | 3600 |
| A | @ | 185.199.110.153 | 3600 |
| A | @ | 185.199.111.153 | 3600 |

**Plus** add a **CNAME record** for www:

| Type | Host | Value | TTL |
|------|------|-------|-----|
| CNAME | www | thenoma.github.io | 3600 |

#### **B. For Subdomain** (e.g., `www.nomausa.org`)

Add **1 CNAME record**:

| Type | Host | Value | TTL |
|------|------|-------|-----|
| CNAME | www | thenoma.github.io | 3600 |

---

## 🔧 Step 3: Configure GitHub Pages

1. **Go to your repository settings**:
   https://github.com/thenoma/NOMA/settings/pages

2. **In the "Custom domain" field**, enter your domain:
   - For apex: `nomausa.org`
   - For www: `www.nomausa.org`

3. **Click "Save"**

4. **Wait 24-48 hours** for DNS propagation (usually takes 1-2 hours)

5. **Check "Enforce HTTPS"** once the domain is verified
   - This may take up to 24 hours to become available
   - Provides free SSL certificate for your custom domain

---

## 📝 Detailed Instructions by Registrar

### Namecheap DNS Setup:

1. Log in to Namecheap
2. Go to Domain List → Click "Manage" next to your domain
3. Go to "Advanced DNS" tab
4. Add the records:
   - Click "Add New Record"
   - Select type (A or CNAME)
   - Enter the host and value from table above
   - Save all changes

### Cloudflare DNS Setup:

1. Log in to Cloudflare
2. Select your domain
3. Go to "DNS" section
4. Click "Add record"
5. Add the A and CNAME records from table above
6. **Important**: Set the proxy status to "DNS only" (gray cloud, not orange)
7. Save

### Google Domains / Squarespace DNS Setup:

1. Log in to your account
2. Go to "My domains"
3. Click on your domain
4. Go to "DNS" section
5. Scroll to "Custom resource records"
6. Add the records from table above
7. Save

---

## 🔍 Step 4: Verify Setup

### Check DNS Propagation:
Visit: https://dnschecker.org
- Enter your domain name
- Select record type (A or CNAME)
- Check if your records are showing up globally

### Test Your Website:
After DNS propagates (1-2 hours, max 48 hours):
- Visit your custom domain
- Should redirect to your NOMA website
- May show "Page not found" initially - this is normal

### Enable HTTPS:
1. After domain is verified (may take 24 hours)
2. Go back to GitHub Pages settings
3. Check "Enforce HTTPS"
4. Wait a few minutes for SSL certificate

---

## 🚨 Troubleshooting

### "Domain is not properly configured"
- Wait longer - DNS takes time to propagate
- Double-check your DNS records match exactly
- Make sure you used `thenoma.github.io` (without /NOMA/)

### "Certificate error" or "Not secure"
- Wait 24 hours after adding custom domain
- Make sure "Enforce HTTPS" is checked
- Try accessing with https:// prefix

### Website shows 404
- Check that your custom domain is spelled correctly
- Verify DNS records are correct
- Clear your browser cache
- Try in incognito mode

### "There isn't a GitHub Pages site here"
- Make sure GitHub Pages is still enabled
- Verify your custom domain is saved in GitHub settings
- Check that you have an `index.html` in the root

---

## 📊 Expected Timeline

| Action | Time |
|--------|------|
| Buy domain | 5-10 minutes |
| Configure DNS | 5-10 minutes |
| DNS propagation | 1-2 hours (max 48h) |
| SSL certificate | 1-24 hours |
| **Total time to live site** | **2-48 hours** |

---

## 💡 Recommended Domain

For NOMA (Network of Moroccans in America), I recommend:

**Primary choice**: `nomausa.org`
- Professional (.org for organizations)
- Clear and memorable
- Represents your mission

**If taken**: `noma-usa.org` or `moroccansinamerica.org`

---

## 🎯 Quick Start Checklist

- [ ] Choose domain registrar (Namecheap recommended)
- [ ] Search for available domain names
- [ ] Purchase domain (~$10-15/year)
- [ ] Add DNS records (4 A records + 1 CNAME)
- [ ] Add custom domain in GitHub Pages settings
- [ ] Wait for DNS propagation (check dnschecker.org)
- [ ] Enable HTTPS in GitHub Pages
- [ ] Test your website!

---

## 📞 Need Help?

If you run into issues:
1. Check the troubleshooting section above
2. Use dnschecker.org to verify DNS
3. GitHub's custom domain docs: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

---

**Remember**: The only recurring cost is the domain name renewal (~$10-15/year). Everything else is FREE! 🎉

