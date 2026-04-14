# Claude Code Instructions

Minimalist static academic personal website. No build system, no frameworks.
Styled after Jon Barron's personal site (jonbarron.info).

## Structure

```
index.html          — single-page site, all content here
stylesheet.css      — all styles (Lato font, #1772d0 links, #f09228 hover)
gilead_poster.pdf   — Gilead Data Discovery poster artifact
bair_paper.pdf      — BAIR Speech Group paper (Pasumarthy, Li et al.)
images/
  Minggang.jpg      — profile photo
  Minggang_Li_CV.pdf
  bair.png          — BAIR logo
  nasa.png          — NASA logo
  visa.png          — Visa logo
  gilead.png        — Gilead Sciences logo
  cpu.svg           — favicon
.nojekyll           — disables Jekyll on GitHub Pages
```

## Local preview

```bash
cd /Users/minggangli/Workspace/my-site
python3 -m http.server 8000
# open http://localhost:8000
```

## Page structure (index.html)

Sections in order:
1. Header — name, intro paragraph, profile photo, inline links (Email / CV / GitHub / LinkedIn)
2. Research — summary paragraph + BAIR entry + NASA entry
3. Experience — Visa entry + Gilead entry
4. Footer — "Last updated April 2026. Design adapted from Jon Barron's website."

## Style conventions

- Font: Lato (loaded via @font-face from Google Fonts CDN in stylesheet.css)
- Body font size: 14px
- Link color: #1772d0 (blue)
- Hover color: #f09228 (orange) — defined in stylesheet.css
- Name heading: .name class, 32px
- Section headings: h2, 22px, font-weight normal
- Entry titles: <strong>, inline
- Roles: <em>, inline
- Dates: <span style="color:#888;font-size:13px;">
- Artifact links: bracket style inline on the title line, e.g. [Paper] [Poster]
- Logo wrapper: width:140px; min-width:140px; display:flex; align-items:center; justify-content:center
- Logo image: max-width:110px; max-height:70px; width:auto; height:auto; object-fit:contain

## Layout

- Outer table: max-width 800px, centered
- Header: two-column table — 63% text / 37% photo, photo is circular (border-radius:50%)
- Entry rows: two-column table — 20% logo / 75% text, border-spacing:0px 6px
- All layout is table-based with inline styles (Barron's approach)

## Updating content

- To update CV: replace images/Minggang_Li_CV.pdf (keep same filename)
- To update BAIR paper: replace bair_paper.pdf (keep same filename)
- To update Gilead poster: replace gilead_poster.pdf (keep same filename)
- Selected Projects section is commented out in index.html — uncomment to restore

## Deployment

GitHub Pages repo: minggangli1030/minggangli1030.github.io
.nojekyll ensures files are served as static HTML without Jekyll processing.
Push to main branch to deploy.
