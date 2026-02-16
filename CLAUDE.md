# CLAUDE.md — Agent Rules for justinbricker.com

## Project Overview

Personal website / digital CV for Justin Bricker. Hosted on GitHub Pages at `www.justinbricker.com`.

## Tech Stack

Plain HTML, CSS, and JavaScript. **No frameworks, no build tools, no package managers.** This is intentional — keep it lightweight.

## File Structure

```
index.html                  # Single-page site (all sections)
css/style.css               # All styles (themes, responsive, layout)
js/main.js                  # Interactivity (dark mode, nav, animations)
CNAME                       # GitHub Pages custom domain
.nojekyll                   # Bypass Jekyll
.github/workflows/deploy.yml  # GitHub Pages deployment
```

## Branching & Deployment

- **Push directly to `main`** for all changes. No PRs needed until the site is live and we are making changes to publicly visible content.
- GitHub Actions deploys to GitHub Pages automatically on push to `main`.
- The `CNAME` file must remain — it controls the custom domain mapping.

## Design Principles

- Minimal, clean, professional aesthetic
- Dark/light mode via `data-theme` attribute on `<html>` and CSS custom properties
- Responsive mobile-first design
- No external dependencies (no CDNs, no Google Fonts, no icon libraries)
- SVG icons are inlined in the HTML
- System font stack (`-apple-system, BlinkMacSystemFont, ...`)

## Code Conventions

- CSS uses custom properties (variables) defined in `:root` and `[data-theme="dark"]` for theming
- CSS class naming: lowercase with hyphens (e.g., `project-card`, `section-title`)
- JavaScript uses IIFEs to avoid polluting global scope
- No transpilation — write browser-compatible JS (no import/export, no optional chaining in older targets)

## Content

- All content is placeholder text until the user provides real details
- Experience, projects, education sections contain template entries showing the expected format
- Social links point to `github.com/justinbricker`, `linkedin.com/in/justinbricker`, and `justin@justinbricker.com` — update if the user provides different URLs

## What NOT to Do

- Do not add npm, yarn, or any package manager
- Do not add a build step (webpack, vite, parcel, etc.)
- Do not add CSS frameworks (Tailwind, Bootstrap, etc.)
- Do not add JS frameworks (React, Vue, etc.)
- Do not add external CDN dependencies
- Do not remove or modify the `CNAME` or `.nojekyll` files without explicit instructions
- Do not create separate HTML pages — this is a single-page site
