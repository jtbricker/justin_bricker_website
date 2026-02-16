# justinbricker.com

Personal website and digital CV for Justin Bricker — Data Engineer, Computational Scientist, and AI Enthusiast based in Nashville, TN.

## Tech Stack

Plain HTML, CSS, and JavaScript. No frameworks, no build step, no external dependencies.

## Structure

```
index.html                     Main single-page site
css/style.css                  Styles, theming, responsive layout
js/main.js                     Dark mode, mobile nav, scroll animations
CNAME                          Custom domain config
.nojekyll                      Bypass Jekyll processing
.github/workflows/deploy.yml   GitHub Pages deployment
CLAUDE.md                      Agent rules for AI-assisted development
```

## Features

- Single-page layout with sections: Hero, About, Experience, Skills, Projects, Education, Contact
- Dark/light mode toggle with system preference detection
- Responsive mobile-first design with hamburger nav
- Scroll-triggered fade-in animations
- No external CDNs, fonts, or icon libraries — everything is self-contained

## Development

Open `index.html` in a browser to preview locally. No install or build step required.

## Deployment

Automatically deployed to GitHub Pages on push to `main` via GitHub Actions.

Custom domain: `www.justinbricker.com`

### Setup

1. **GitHub Pages**: repo Settings > Pages > Source: GitHub Actions
2. **DNS**: `CNAME` record `www` -> `jtbricker.github.io`, plus `A` records for apex domain ([GitHub docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site))
3. **HTTPS**: Enable "Enforce HTTPS" in Pages settings
