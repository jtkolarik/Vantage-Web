# Vantage Studio Website

Single-page marketing site for Vantage Studio, built with Astro and Tailwind CSS.

## Quick Start

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Deployment to Netlify

### Option 1: Deploy via Netlify CLI

```bash
# Install Netlify CLI
npm install -g netlify-cli

# Login to Netlify
netlify login

# Deploy (creates new site)
netlify deploy --prod
```

### Option 2: Connect Git Repository

1. Push this project to a Git repository (GitHub, GitLab, or Bitbucket)
2. Log in to [Netlify](https://app.netlify.com)
3. Click "Add new site" > "Import an existing project"
4. Connect your Git provider and select the repository
5. Build settings will be auto-detected from `netlify.toml`
6. Click "Deploy site"

### Custom Domain

1. In Netlify dashboard, go to "Domain settings"
2. Add custom domain: `vantage-studio.com`
3. Follow DNS configuration instructions

## Project Structure

```
/
├── public/
│   ├── images/
│   │   ├── hero-porch.png
│   │   ├── contrails.png
│   │   ├── porch-night.png
│   │   └── portfolio/
│   │       ├── noble.png
│   │       ├── redemption.png
│   │       └── rydell.png
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Hero.astro
│   │   ├── Services.astro
│   │   ├── Portfolio.astro
│   │   ├── About.astro
│   │   ├── Contact.astro
│   │   └── Footer.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── netlify.toml
└── tailwind.config.js
```

## Portfolio Screenshots

To add portfolio screenshots:

1. Capture above-the-fold screenshots from each site:
   - https://noblecontracting.netlify.app/
   - https://redemptionelectric.netlify.app/
   - https://rydell.netlify.app/

2. Save as `noble.png`, `redemption.png`, and `rydell.png` in `public/images/portfolio/`

3. Recommended dimensions: 1600x1000px or similar 16:10 aspect ratio

## Contact Form

The contact form uses Netlify Forms. After deploying:

1. Netlify will automatically detect the form
2. Submissions appear in Netlify dashboard > Forms
3. Configure email notifications in Form settings

## Brand Colors

- Navy (primary bg): `#0a1628`
- Twilight (secondary): `#1a3a5c`
- Amber (accent): `#d4a574`
- Orange (hover): `#e8945a`
- Cream (text): `#f5f0e8`
- Wheat (subtle): `#c9b896`
