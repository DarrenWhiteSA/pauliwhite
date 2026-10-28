# Pauli White | sensory gardens

Single-page website for Pauli White's garden design practice in Cape Town. Static HTML with no build step; deploys to Netlify as-is (`netlify.toml` publishes the repo root and redirects the old `/luxury/` page here).

Sections: 01 Introduction · 02 Approach (Structure. Senses. Self.) · 03 Process · testimonial bar · 04 Contact.

## Brand

Taken from Pauli's "Pauli White | Sensory Gardens" advertisement:

- `images/pw-mark.png`: the flower mark, extracted from the advertisement as white on transparent. The page recolours it with a CSS mask (`.mark`), so it can be olive on ivory or ivory on olive without a second file.
- `images/pw-leaves-intro.jpg`, `images/pw-leaves-contact.jpg`: crops of the watercolour leaf artwork, with no lettering.
- `images/pw-brand-artwork.jpg`: the advertisement artwork, used as the social-share image.
- Colours (sampled from the advertisement): ivory `#ece8dd`, olive `#636131`, deep olive `#4a4524`, moss `#6d6a3a`, charcoal `#2f2e29`.
- Type: Cormorant Garamond (headings and the widely spaced wordmark) and Jost (the "sensory gardens" descriptor and body text).

## Editing

- **Approach images:** one each for Structure, Senses and Self. Keep each caption honest: label concept renders as renders.
- **Testimonials:** add genuine quotes to the `TESTIMONIALS` list in the page script. The bar stays hidden while the list is empty, and rotates one quote at a time once there is more than one.
- **Fees:** the concept fee and the deposit split are in the Process section.

## Preview locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000.
