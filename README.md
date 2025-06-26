# Yamnesh Agrawal - Academic Website

A modern, responsive academic website for PhD student Yamnesh Agrawal, showcasing research interests, publications, and professional information.

## Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional design with smooth animations
- **Interactive Navigation**: Smooth scrolling and active section highlighting
- **Contact Form**: Integrated contact form that opens the user's email client
- **Google Scholar Integration**: Links to Google Scholar profile with placeholder for citation stats
- **Research Showcase**: Dedicated sections for research areas and interests
- **Professional Branding**: Consistent color scheme and typography

## Sections

1. **Hero Section**: Introduction with name, title, and key information
2. **About**: Personal background, education, and research areas
3. **Research**: Detailed research interests and focus areas
4. **Publications**: Link to Google Scholar profile and citation metrics
5. **Contact**: Contact information and form

## File Structure

```
Website/
├── index.html          # Main HTML file
├── styles.css          # CSS styles and responsive design
├── script.js           # JavaScript for interactivity
└── README.md          # This file
```

## Customization

### Personal Information
Edit the following in `index.html`:
- Replace placeholder profile image URL in the hero section
- Update education details in the about section
- Add your LinkedIn, ResearchGate, and other social media links
- Modify research descriptions to match your specific work

### Contact Information
- Email: Currently set to `yamnesh@pitt.edu`
- Institution: University of Pittsburgh, Department of Mechanical Engineering & Material Science
- Google Scholar: Link is already configured

### Colors and Styling
The website uses a purple gradient theme. To customize colors, edit the CSS variables in `styles.css`:
- Primary color: `#4f46e5` (Indigo)
- Secondary color: `#7c3aed` (Purple)
- Background gradients and accent colors

### Adding Publications
To add actual publications:
1. Replace the placeholder content in the publications section
2. Consider integrating with Google Scholar API (requires backend implementation)
3. Add individual publication items in the publications list

## Browser Compatibility

- Chrome/Edge/Safari: Full support
- Firefox: Full support
- Internet Explorer: Basic support (CSS Grid fallbacks included)

## Performance Features

- Optimized images and lazy loading
- Debounced scroll events
- Smooth animations with hardware acceleration
- Minimal external dependencies

## Deployment

### Option 1: GitHub Pages
1. Push the files to a GitHub repository
2. Enable GitHub Pages in repository settings
3. Your site will be available at `https://yourusername.github.io/repository-name`

### Option 2: Netlify (Recommended)
1. Create account at netlify.com
2. Drag and drop the Website folder
3. Get instant HTTPS deployment with custom domain support

### Option 3: Traditional Web Hosting
Upload all files to your web hosting provider's public folder (usually `public_html` or `www`)

## Adding Dynamic Features

### Backend Integration
For advanced features like:
- Contact form that sends emails directly
- Real-time Google Scholar citation fetching
- Content management system

Consider adding:
- Node.js/Express backend
- Python Flask/Django backend
- Serverless functions (Netlify Functions, Vercel Functions)

### Analytics
Add Google Analytics by including the tracking code in the `<head>` section of `index.html`

## Maintenance

### Regular Updates
- Update publications and achievements
- Refresh research descriptions
- Update contact information as needed
- Add new sections (e.g., Teaching, Awards, News)

### SEO Optimization
- Add meta descriptions and keywords
- Include structured data for academic profiles
- Optimize images with alt tags
- Submit sitemap to search engines

## Technical Notes

- Uses CSS Grid and Flexbox for layouts
- Implements Intersection Observer API for animations
- Responsive breakpoints: 768px (tablet), 480px (mobile)
- Font: Inter from Google Fonts
- Icons: Font Awesome 6

## Support

For technical issues or customization help:
1. Check browser developer console for errors
2. Validate HTML/CSS using W3C validators
3. Test on multiple devices and browsers

## License

This website template is provided as-is for academic use. Feel free to modify and customize according to your needs.

---

**Note**: Remember to replace placeholder content with your actual information and add a professional headshot to complete your academic website.
