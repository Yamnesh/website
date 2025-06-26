# Custom Domain Setup Guide for Spaceship + Vercel

## Your Domain Configuration

### Step 1: Vercel Dashboard Setup
1. Go to [vercel.com/dashboard](https://vercel.com/dashboard)
2. Click on your project: `yamnesh-academic-website`
3. Navigate to: Settings → Domains
4. Click "Add Domain" and enter your domain name

### Step 2: Spaceship DNS Configuration

#### Method 1: DNS Records (Recommended)
Log into your Spaceship account and add these DNS records:

**For Root Domain (yourdomain.com):**
```
Type: A
Name: @ (or blank)
Value: 76.76.19.61
TTL: 3600 (or Auto)

Type: CNAME
Name: www
Value: cname.vercel-dns.com
TTL: 3600 (or Auto)
```

**For WWW Only (www.yourdomain.com):**
```
Type: CNAME
Name: www
Value: cname.vercel-dns.com
TTL: 3600 (or Auto)
```

#### Method 2: Use Vercel Nameservers (Easier)
If you prefer Vercel to manage your DNS:

1. In Vercel, select "Use Vercel nameservers"
2. Copy the provided nameservers (usually):
   - ns1.vercel-dns.com
   - ns2.vercel-dns.com
3. In Spaceship, update your domain's nameservers to these

### Step 3: Verification
- DNS propagation: 15 minutes to 48 hours
- Check status in Vercel dashboard
- SSL certificate will be issued automatically

### Step 4: Testing
Once propagation is complete:
- Visit your custom domain
- Verify HTTPS is working
- Test on multiple devices

## Troubleshooting

### Common Issues:
1. **DNS not propagating**: Wait longer, check with online DNS checker tools
2. **Certificate issues**: Usually resolves automatically after DNS propagation
3. **Mixed content warnings**: Ensure all resources use HTTPS

### Verification Tools:
- [whatsmydns.net](https://whatsmydns.net) - Check DNS propagation
- [dnschecker.org](https://dnschecker.org) - Global DNS checker
- Browser developer tools - Check for any errors

### Support:
- Vercel: [vercel.com/support](https://vercel.com/support)
- Spaceship: Check their support documentation

## Domain Best Practices

### Security:
- Enable domain lock in Spaceship
- Set up domain privacy protection
- Use strong passwords for domain account

### Performance:
- Use both www and non-www versions
- Redirect one to the other for consistency
- Monitor loading speeds after DNS changes

### SEO:
- Set up Google Search Console with your custom domain
- Submit new sitemap with custom domain
- Update any existing links to use new domain

---

**Remember**: After DNS propagation, your academic website will be live at your custom domain with automatic HTTPS!
