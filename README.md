# Pauli White — Sensory landscape design

Static one-page site for Pauli White's landscape design and services business. No build step; deploys to Netlify as-is (`netlify.toml` publishes the repo root).

## Design system

Carried over from Pauli's CV site (cv-pauli-white.netlify.app) so the two read as one identity:

- Colour tokens in `:root` at the top of `index.html`: paper `#ffffff`, warm paper `#faf9f7`, sage `#adbba1`, deep sage `#7d8b73`, stone `#c7c8be`, ink `#3a3e38`, soft ink `#6e736b`, rule `#e2e3de`.
- Type: Jost (200–400) for everything, Cormorant Garamond italic for quotes and emphasis.
- Restrained headings, thin rules, generous whitespace.

## Variant B: Landscape Studio (`luxury/`)

A second design direction at `/luxury/`, aimed at estates, hotels, wine farms and schools. It deliberately departs from the CV identity:

- Palette: night `#1b1f1a`, moss `#2c3428`, bone `#f2ede3`, brass `#a8865a`.
- Type: Bodoni Moda (display, with italic emphasis) and Manrope (body).
- Layout: full-bleed hero, a sectors index, alternating case-study features with the concept sketch inset over the finished image, a project index table, and a lightbox (`GALLERIES` in the page script).

It shares the `images/` folder with the main page.

## Adding a project

1. Put the image files in `images/` (about 1400px wide, JPEG).
2. Add an entry to the `PROJECTS` array in the `<script>` near the bottom of `index.html`: `title`, `kind` (type and year), `cover`, `note`, `summary`, `facts` and `images`. Set `wide:true` for a full-width card and `two:true` for a two-column gallery in the drawer.

## Preview locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000.
