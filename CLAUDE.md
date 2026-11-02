# The Wow Style — project instructions

Fashion and outfit-ideas site: thewowstyle.co.uk. Styling guides for men and
women. Launch state is one section, **How to Style**, with 30 guides.

## Standing instruction — image prompt pack with every article

**Whenever an article is written, end it with a ChatGPT image prompt pack** —
but only when asked for it. Do not append one unprompted.

The pack must state, for that specific article:

| Item | What to give |
|---|---|
| **How many images** | Total count for the article, broken down by type (hero, looks, detail crops, pins) |
| **Featured image** | One featured image at 1200×700, exported as WebP (`.webp`) |
| **Variations** | Which model, and how many images each |
| **Outfits** | A written outfit line per image — garment, colour, fabric, fit **and the shoes** |
| **Accessories** | A different accessory per image, or none — never the same one (e.g. a watch) in every image |
| **Poses** | A different pose per image, rotated, never repeating consecutively |
| **Face angle** | A different face angle per image (straight, three-quarter, over-the-shoulder, tilted), never the same twice in one guide |
| **Background** | A different background colour per image, never the same twice in one guide |
| **Details** | One small imperfection per image |
| **Framing & format** | Per image: full body / three-quarter / waist-up / low angle / detail crop, and 2:3 or 3:4 |
| **Alt text** | A written alt text per image — the outfit described, with the keyword where natural |
| **Section / placement** | Which section of the article each image goes in |
| **Filenames** | The exact path each file saves to, matching the article slug |

Write it so it can be pasted into ChatGPT one block at a time with no assembly.

**Default image style is the mirror-selfie + flat-lay** (the phone covers the face, so
no reference photo is needed and the model can't drift). Use it for every article image:
- `MIRROR-SELFIE-FLATLAY-PROMPT.md`

Face-locked portraits — only for images where a face IS shown (e.g. an author portrait):
- `FEMALE-MODEL-PROMPT.md`
- `MALE-MODEL-PROMPT.md`

Keep these files in sync if a model's look changes.

## Image rules that apply everywhere

- **The default style hides the face (the phone covers it), so no reference photo is
  needed and the model can't drift.** Only when an image actually shows a face (e.g. an
  author portrait) must the reference photo be attached to every ChatGPT message.
- **Give every image a different background colour** — a different plain studio-wall
  colour — so no two images in a guide or on a page share one. Keep the lighting soft,
  natural daylight and the colour grade natural.
- **Vary the pose and phone position every image** — the face is hidden, so there is no
  face angle to vary. (For any face-shown image, vary the face angle instead.)
- **Every article has a featured image at 1200×700, saved as WebP** (`.webp`).
- **Orientation:** outfit/look images and Pinterest pins are vertical 2:3 (1000×1500);
  the featured image is horizontal 1200×700.
- **Watermark every image with `thewowstyle.co.uk`** — added *after* generation (a
  WordPress watermark plugin or a batch step), never drawn by the AI. Small, bottom-right,
  ~55% opacity. The AI prompt still says no text/watermark, so the model never renders
  text itself.
- Every outfit line names the shoes.
- Audience panels crop to the bottom quarter behind a caption — frame those from
  the knee up.
- Inside an article the shoes must be visible.
- Never reuse one photograph in two slots on the same page.

## Site files

| File | Purpose |
|---|---|
| `index.html` | Homepage, production. Loads from `images/` |
| `preview.html` | Same page with images inlined, for viewing only |
| `images/` | Live photographs |
| `TheWowStyle_120_Article_Roadmap.xlsx` | 120 articles, 7 pillars, zero topic overlap |

## Content and SEO conventions

- Permalinks: `/how-to-style/<slug>/` — one category level, no dates
- Article titles 60 characters or fewer
- Slugs are the primary keyword only, set by hand, never WordPress's default
- Internal links: one up to the pillar in the first 150 words, 2-3 siblings in the
  same pillar, cross-pillar only where a shared term makes it natural
- Guides are image-led: 25-40 images, 900-1,400 words
- Affiliate disclosure sits above the first affiliate link, not in the footer
