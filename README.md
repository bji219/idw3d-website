# Intelligent Design Works Limited - Business Website

Official website for Intelligent Design Works Limited, featuring custom audio equipment innovations and accessories for musicians and audio enthusiasts.

## About

Intelligent Design Works specializes in precision-engineered solutions for audio enthusiasts, including:
- Display systems (Zero-G Record Display System)
- Accessories (Retro Analog Synth Knobs for OP-1)
- Stands & Risers (OP-1 x Korg SV-Series Synth Riser)
- Custom modifications (OP-1F Retrofuturistic Side Plates)

## Technology Stack

This is a static website built with:
- Pure HTML5
- Embedded CSS3 with modern animations and responsive design
- Google Fonts (DM Mono, Syne)
- No build process required

## Deployment

### Netlify Setup

This repository is configured for automatic deployment on Netlify.

#### Quick Start:

1. **Connect to Netlify:**
   - Log in to [Netlify](https://www.netlify.com/)
   - Click "Add new site" > "Import an existing project"
   - Connect to your Git provider and select this repository
   - Netlify will automatically detect the settings from `netlify.toml`

2. **Automatic Deployment:**
   - Every push to your main branch will trigger a new deployment
   - Preview deployments are created for pull requests

3. **Configuration:**
   All deployment settings are defined in `netlify.toml`:
   - No build command needed (static HTML)
   - Publishes from root directory (.)
   - Security headers configured
   - Smart redirects enabled

### Custom Domain

To connect a custom domain:
1. Go to Site settings > Domain management in Netlify
2. Add your custom domain
3. Update your DNS settings as instructed by Netlify

### Environment Variables

This site doesn't require any environment variables. All content is static.

## Local Development

To view the site locally:

1. Simply open `index.html` in a web browser
2. Or use a local server:
   ```bash
   # Python 3
   python -m http.server 8000

   # Node.js (if you have npx)
   npx serve
   ```

Then visit `http://localhost:8000` in your browser.

## File Structure

```
idw3d-website/
├── index.html          # Main website file
├── netlify.toml        # Netlify configuration
├── .gitignore          # Git ignore rules
└── README.md           # This file
```

## Features

- **Responsive Design:** Mobile-first approach with breakpoints for all devices
- **Animated Grid Background:** Dynamic visual effects
- **Smooth Animations:** Fade-ins and transitions for enhanced UX
- **Product Showcase:** Grid layout featuring current inventory
- **SEO Optimized:** Proper meta tags and semantic HTML
- **Performance:** Lightweight, fast-loading static site

## Customization

To update content:
1. Edit `index.html` directly
2. Product information, contact details, and links are all inline
3. Update the Etsy shop URL placeholder: `https://www.etsy.com/shop/YourShopName`
4. Commit and push - Netlify will automatically deploy

## Support

For questions or issues with the website, contact: contact@intelligentdesignworks.com

## License

© 2026 Intelligent Design Works Limited. All rights reserved.
