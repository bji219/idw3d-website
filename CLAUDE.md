# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static website for Intelligent Design Works Limited (IDW3D), a company selling custom 3D-printed audio equipment and accessories. Deployed on Netlify with automatic deployments on push to main.

## Local Development

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve
```

Then visit http://localhost:8000

## Architecture

**Single-page static site** with no build process:
- `index.html` - Complete website including all HTML, embedded CSS, and inline styles
- All styling uses CSS custom properties defined in `:root` for theming (--primary-dark, --accent-cyan, --accent-amber, etc.)
- Google Fonts: DM Mono (body) and Syne (headings)
- Responsive design with mobile breakpoint at 768px

## Deployment

Configured in `netlify.toml`:
- Publishes from root directory
- No build command required
- Security headers and caching rules pre-configured
- Automatic deploys on push to main branch

## Key Conventions

- Product cards follow a consistent structure: tag, name, description, features list, and link
- Color scheme: dark background (#0a0e12), cyan accent (#00d9ff), amber accent (#ffb800)
- "Coming Soon" products use the `.coming-soon` class for badge styling
