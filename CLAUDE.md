# CLAUDE.md — Agent Rules for justinbricker.com

## Project Overview

Personal website / digital CV for Justin Bricker — Software Engineer, Data Scientist, and Machine Learning specialist. Hosted on GitHub Pages at `www.justinbricker.com`. Linked from a consulting firm website, so it must be client-presentable.

## Tech Stack

Plain HTML, CSS, and JavaScript. **No frameworks, no build tools, no package managers.** This is intentional — keep it lightweight.

## File Structure

```
index.html                  # Single-page site (all sections)
css/style.css               # All styles (Slate theme, responsive)
js/main.js                  # Interactivity (dark mode, nav, animations)
mockups/                    # Design mockups (SVG + DESIGN.md)
CNAME                       # GitHub Pages custom domain
.nojekyll                   # Bypass Jekyll
.github/workflows/deploy.yml  # GitHub Pages deployment
```

## Branching & Deployment

- **Push directly to `main`** for all changes. No PRs needed until the site is live and we are making changes to publicly visible content.
- GitHub Actions deploys to GitHub Pages automatically on push to `main`.
- The `CNAME` file must remain — it controls the custom domain mapping.

## Design: "Slate" Theme

The site uses the **Slate** design — a dark-first, monospace-forward aesthetic softened for professional/client-facing use:

- **Dark-first**: Default theme is dark (`data-theme="dark"`), with a polished light mode available
- **Monospace typography** for headings, nav, tags, dates, and UI elements (`SF Mono`, `Fira Code`, etc.)
- **Sans-serif** for body text (system font stack)
- **Sharp edges**: 4px border-radius on cards (not rounded), 2px on tags
- **Color palette**: GitHub dark colors (#0d1117 bg, #c9d1d9 text, #58a6ff accent, #30363d borders)
- **No terminal cosplay**: No `$ whoami` prompts or command-line metaphors — keep it professional
- **Responsive mobile-first design**
- **No external dependencies** (no CDNs, no Google Fonts, no icon libraries)
- SVG icons are inlined in the HTML

## Code Conventions

- CSS uses custom properties defined in `:root` (dark) and `[data-theme="light"]` for theming
- CSS class naming: lowercase with hyphens (e.g., `project-card`, `section-title`)
- JavaScript uses IIFEs to avoid polluting global scope
- No transpilation — write browser-compatible JS (no import/export, no optional chaining)

## Content

- Content is based on Justin's real LinkedIn profile
- Social links: `github.com/jtbricker`, `linkedin.com/in/justinbricker`, `jbricker4@gmail.com`
- Experience includes: AcuityMD, Eventbrite, University of Florida (ML Consultant), Infinite Energy, FSU
- Education: M.S. Computational Science (FSU), B.S. Mathematics (UF)
- Publication: AID-P (Parkinsonism imaging differentiation)

## What NOT to Do

- Do not add npm, yarn, or any package manager
- Do not add a build step (webpack, vite, parcel, etc.)
- Do not add CSS frameworks (Tailwind, Bootstrap, etc.)
- Do not add JS frameworks (React, Vue, etc.)
- Do not add external CDN dependencies
- Do not add terminal/command-line metaphors — this site is client-facing
- Do not remove or modify the `CNAME` or `.nojekyll` files without explicit instructions
- Do not create separate HTML pages — this is a single-page site
