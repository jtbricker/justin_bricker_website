# Slate

## Concept

Terminal-inspired, developer-centric design. Dark background, monospace typography, sharp edges, and a single accent color. The vibe is "someone who lives in the terminal built their portfolio."

## Color Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Background | `#0d1117` | Primary background (GitHub dark) |
| Surface | `#161b22` | Card backgrounds, elevated surfaces |
| Border | `#30363d` | All borders, dividers, card outlines |
| Text Primary | `#c9d1d9` | Headings, body text |
| Text Muted | `#8b949e` | Secondary text, nav links, descriptions |
| Text Dim | `#484f58` | Dates, metadata, subtle labels |
| Accent | `#58a6ff` | Links, markers, highlights, interactive elements |

## Typography

- **All text**: Monospace system stack (`SF Mono`, `Fira Code`, `Fira Mono`, `Roboto Mono`, `monospace`)
- **Headings**: Prefixed with `#` like code comments, bold weight
- **Body**: Regular weight monospace
- **Dates/metadata**: Smaller size, dim color
- **Tags**: Prefixed with `#` like hashtags, accent color

## Layout

- Single column, max-width ~960px, centered
- Generous vertical spacing between sections (80-100px)
- Horizontal rule dividers between sections (thin, border color)
- No rounded corners anywhere — all sharp/square edges
- Consistent left-alignment throughout

## Key Design Elements

- Section headings prefixed with `#` like code comments
- CTA styled as a terminal command: `> view_my_work`
- Hero has a `$ whoami` prompt above the name
- Contact section styled as terminal output (`$ echo $EMAIL`)
- Social links are square-bordered boxes with text abbreviations, not icons
- Skill tags are rectangular bordered elements (no fill, border only)
- Project cards have sharp corners with thin borders on dark surface
- Timeline uses simple circles and a vertical line
- Blinking cursor element in the hero section
- Footer minimal — could show `$ exit`

## Navigation

- Flat text links in monospace, spaced evenly on the right
- Logo "JB" on the left in accent color
- Thin bottom border separating nav from content
- No background fill — transparent over the dark background
- `[light]` / `[dark]` toggle styled as a terminal bracket option

## Dark / Light Mode

- **Dark-first design** — the dark theme is the primary, defining aesthetic
- Light mode inverts: white background, dark text, but keeps monospace and sharp edges
- Light mode accent shifts to a darker blue for contrast
- The terminal metaphor carries through both modes but feels most natural in dark

## Sections

- **Hero**: `$ whoami` prompt, large monospace name, pipe-separated subtitle, square social boxes, terminal-command CTA
- **About**: `# about` heading, monospace paragraph text, no decorative elements
- **Experience**: Vertical timeline with dots and connecting line, entries with role/company/date
- **Skills**: Category labels in uppercase dim text, skills as bordered rectangular tags (no fill)
- **Projects**: 2-column grid of sharp-cornered cards on dark surface, `[src]` link in corner, `#tech` tags at bottom
- **Education**: Similar to experience entries, minimal
- **Contact**: Terminal-output style with `$` prompts and command-like formatting

## Mood / Inspiration

Communicates technical depth and comfort with the command line. Signals that this person is a builder who values efficiency and substance over flash. The GitHub-dark palette feels immediately familiar to developers. The monospace-everywhere choice is polarizing by design — it says "I know my audience, and my audience lives in terminals and code editors."
