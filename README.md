# justinbricker.com

Personal website and digital CV for Justin Bricker — Data Engineer, Computational Scientist, and AI Enthusiast based in Nashville, TN.

## Tech Stack

Plain HTML, CSS, and JavaScript. No frameworks, no build step.

## Development

Open `index.html` in a browser to preview locally.

## Deployment

Automatically deployed to GitHub Pages on push to `main` via GitHub Actions. Custom domain: `www.justinbricker.com`.

### DNS Setup

Point your domain to GitHub Pages:
- `CNAME` record: `www` -> `<username>.github.io`
- `A` records for apex domain -> GitHub Pages IPs (see [GitHub docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site))

### GitHub Pages Setup

1. Go to repo Settings > Pages
2. Source: GitHub Actions
3. Custom domain: `www.justinbricker.com`
4. Enforce HTTPS: enabled
