# VijayKas-Portfolio

Personal portfolio website for Vijay Kas — **vijaykas.com**

## Tech Stack

- Plain HTML + CSS + vanilla JS (no frameworks)
- Deployed via Cloudflare Workers (static assets)
- Domain: vijaykas.com (GoDaddy → Cloudflare nameservers)

## Design System

**Style**: Light clean + editorial — typography-forward, minimal, professional

### Colors
| Token      | Value     | Usage                  |
|------------|-----------|------------------------|
| Background | `#F8F7F4` | Page background        |
| Text       | `#1A1A1A` | Primary text           |
| Accent     | `#2563EB` | Links, highlights      |
| Muted      | `#6B7280` | Secondary text, labels |

### Typography
- **Headings**: Playfair Display (serif, Google Fonts)
- **Body**: Source Sans 3 (sans-serif, Google Fonts)
- **Labels/Counters**: IBM Plex Mono (monospace, Google Fonts)
- Fluid sizing via `clamp()`

### Layout
- Single-page with anchor navigation
- Mobile-first responsive
- Smooth scroll (`scroll-behavior: smooth`)
- Scroll-reveal animations (Intersection Observer)
- `prefers-reduced-motion` respected

## Sections
1. **Hero** — Name, role, tagline, page-load animation
2. **About** — Bio, photo placeholder, key strengths
3. **Ventures** — ZunicLabs / BatchBook with descriptions
4. **Projects** — Project highlights in card layout
5. **Blog** — Links to blog listing page
6. **Contact** — Email, LinkedIn, GitHub

## File Structure
```
VijayKas-Portfolio/
├── index.html
├── blog/
│   └── index.html
├── wrangler.jsonc
├── .gitignore
├── .nvmrc
└── AGENTS.md
```

## Deployment
- Cloudflare Workers with `assets.directory` pointing to `.` (root)
- Separate Cloudflare account from zuniclabs@gmail.com
- Git push → manual deploy via wrangler (auto-deploy TBD)
