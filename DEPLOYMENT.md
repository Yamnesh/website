# Deployment Guide for Your Academic Website

## Quick Start - Local Testing

1. **Run the local server:**
   ```bash
   cd /Users/yamnesh/Documents/Python/Website
   python3 serve.py
   ```
   This will start a local server and automatically open your website in your browser.

2. **Alternative local server:**
   ```bash
   cd /Users/yamnesh/Documents/Python/Website
   python3 -m http.server 8000
   ```
   Then visit http://localhost:8000

## Deployment Options

### 1. GitHub Pages (Free & Easy)

**Steps:**
1. Create a new repository on GitHub (e.g., `your-academic-website`)
2. Upload all files from your Website folder
3. Go to repository Settings → Pages
4. Select "Deploy from a branch" → "main" → "/ (root)"
5. Your site will be live at `https://yourusername.github.io/your-academic-website`

**Advantages:**
- Free hosting
- Custom domain support
- Automatic HTTPS
- Version control with Git

### 2. Netlify (Recommended)

**Steps:**
1. Visit [netlify.com](https://netlify.com) and create account
2. Drag and drop your Website folder to Netlify
3. Get instant deployment with custom URL
4. Optional: Connect your domain

**Advantages:**
- Fastest deployment
- Excellent performance
- Form handling capabilities
- Free SSL certificates

### 3. Vercel

**Steps:**
1. Visit [vercel.com](https://vercel.com) and sign up
2. Connect your GitHub repository
3. Automatic deployments on code changes

### 4. Traditional Web Hosting

Upload files to any web hosting provider:
- Bluehost, SiteGround, HostGator, etc.
- Upload to public_html or www folder
- Configure domain settings

## Customization Checklist

Before deployment, customize these elements:

### Essential Updates
- [ ] Replace placeholder profile image
- [ ] Update education details with your specific information
- [ ] Add your actual research publications
- [ ] Update social media links (LinkedIn, ResearchGate, etc.)
- [ ] Verify email contact information

### Optional Enhancements
- [ ] Add Google Analytics tracking
- [ ] Include your CV/Resume download link
- [ ] Add a blog/news section
- [ ] Include teaching experience
- [ ] Add awards and achievements section

## SEO Optimization

Add these to your `index.html` `<head>` section:

```html
<meta name="description" content="Yamnesh Agrawal - PhD Student in Mechanical Engineering & Material Science at University of Pittsburgh. Research in soft tissue biomechanics, wave propagation, and non-destructive evaluation.">
<meta name="keywords" content="Yamnesh Agrawal, PhD student, mechanical engineering, biomechanics, wave propagation, University of Pittsburgh">
<meta name="author" content="Yamnesh Agrawal">

<!-- Open Graph (Social Media) -->
<meta property="og:title" content="Yamnesh Agrawal - PhD Student">
<meta property="og:description" content="PhD Student in Mechanical Engineering & Material Science">
<meta property="og:type" content="website">
<meta property="og:url" content="https://yourdomain.com">
```

## Domain Setup

### Free Options
- GitHub Pages: `yourusername.github.io/repository-name`
- Netlify: `random-name.netlify.app` (can customize)

### Custom Domain
1. Purchase domain from:
   - Namecheap, GoDaddy, Google Domains
   - Recommended: `.com` or `.edu` if available through your institution

2. Configure DNS:
   - Point domain to your hosting provider
   - Enable HTTPS (usually automatic)

## Maintenance

### Regular Updates
- Update publications quarterly
- Refresh research descriptions
- Add new achievements and awards
- Keep contact information current

### Performance Monitoring
- Use Google PageSpeed Insights
- Monitor loading times
- Optimize images if needed
- Update dependencies annually

## Security Considerations

### Contact Form
Current form opens email client. For direct form submission:
- Use Netlify Forms (free tier available)
- Implement server-side processing
- Add CAPTCHA for spam protection

### HTTPS
- Always use HTTPS (enabled by default on modern platforms)
- Keep dependencies updated
- Regular security scans

## Analytics Setup

### Google Analytics 4
Add this to your `<head>` section:

```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

Replace `GA_MEASUREMENT_ID` with your actual Google Analytics ID.

## Troubleshooting

### Common Issues
1. **Images not loading**: Check file paths and case sensitivity
2. **CSS not applying**: Clear browser cache, check file paths
3. **Mobile responsiveness**: Test on multiple devices
4. **Form not working**: Verify email links and form action

### Testing Checklist
- [ ] Test on Chrome, Firefox, Safari
- [ ] Test on mobile devices
- [ ] Check all links work
- [ ] Verify contact form functionality
- [ ] Test loading speed
- [ ] Validate HTML/CSS

## Support Resources

- **W3C HTML Validator**: https://validator.w3.org/
- **W3C CSS Validator**: https://jigsaw.w3.org/css-validator/
- **Google PageSpeed Insights**: https://pagespeed.web.dev/
- **Can I Use**: https://caniuse.com/ (browser compatibility)

---

**Ready to deploy?** Start with the local server test, then choose your preferred deployment method above!
