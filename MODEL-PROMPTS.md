# Model Prompt Kit — The Wow Style

Two locked models. Same face, same room, same light in every image, with only the
outfit changing. Copy a block, swap the outfit line, done.

---

## HOW TO ACTUALLY GET CONSISTENCY (read this first)

**Text alone will not hold a face.** ChatGPT, Midjourney and the rest redraw the
person from scratch each time. A written description keeps the *type* of person
consistent, not the person.

So every single generation works like this:

1. **Attach the reference photo** of that model to the message. Every time. Not
   once at the start of a chat — every message.
2. Paste the block below underneath it.
3. Start the message with: **"Keep the exact same face, hair and body from the
   attached photo. Change only the clothing."**

Without step 1 you will get a different person who merely looks similar.

**Two more things that help:**

- Keep one long chat per model rather than starting fresh each time. The chat
  carries the earlier images as context.
- When you get an image you are happy with, save it and use **that** as the new
  reference. Quality drifts if you keep re-referencing the original.
- If a face starts drifting, go back to the original reference and start again.

---

## MODEL A — FEMALE

### Character lock (never change these words)

> Woman in her late twenties. Light olive skin with a warm undertone and natural
> texture — visible pores, no retouching gloss. Dark chestnut-brown hair, shoulder
> length, blunt cut, straight with a soft natural wave, centre-parted, worn loose.
> Oval face, defined dark eyebrows, brown eyes, straight nose, full lips, neutral
> relaxed mouth. Slim build, average height, narrow shoulders. Minimal makeup —
> groomed brows, bare skin, no lipstick. One fine gold chain necklace.

### Full prompt template

```
Keep the exact same face, hair and body from the attached photo.
Change only the clothing.

SUBJECT: Woman in her late twenties. Light olive skin, warm undertone, natural
skin texture. Dark chestnut-brown hair, shoulder length, blunt cut, straight with
a soft wave, centre-parted, loose. Oval face, defined dark brows, brown eyes, full
lips, relaxed neutral expression. Slim build, narrow shoulders. Minimal makeup.

OUTFIT: [YOUR OUTFIT HERE]

POSE: Standing, straight to camera, weight on one leg, arms relaxed at her sides,
looking directly at the lens.

SETTING: Plain warm-grey studio wall, pale oak floor.

LIGHT: Large soft window light from camera left, gentle falloff to the right,
soft shadow under the feet. Daylight, no flash.

CAMERA: Full body, head to shoes, nothing cropped. Shot on 85mm at f/4, eye level,
slight distance so proportions are natural.

STYLE: Editorial fashion photography. Natural colour, no heavy grading, no beauty
retouching. Garments must drape realistically with visible fabric weight and
natural creasing.

FORMAT: Vertical 2:3.

AVOID: Changing the face. Altering hair length or colour. Cartoon or 3D render
look. Plastic skin. Extra fingers. Logos or brand names. Text or watermarks.
Harsh flash. Heavy makeup. Cropping the feet.
```

---

## MODEL B — MALE

### Character lock (never change these words)

> Man in his mid twenties, mixed race, medium-brown skin with a warm undertone and
> natural texture. Dark brown tightly curled hair, short at the sides, a few inches
> of loose curls on top, natural shape. Thin round wire-frame glasses in pale gold
> metal. Light facial hair — a fine moustache and a small chin beard, neatly kept.
> Small stud earring in one ear. Oval face, dark brown eyes, calm neutral
> expression. Slim build, average height, narrow frame.

### Full prompt template

```
Keep the exact same face, hair, glasses and body from the attached photo.
Change only the clothing.

SUBJECT: Man in his mid twenties, mixed race, medium-brown skin with a warm
undertone and natural texture. Dark brown tightly curled hair, short at the sides,
a few inches of loose curls on top. Thin round pale-gold wire-frame glasses. Fine
moustache and a small neat chin beard. Small stud earring. Calm neutral expression.
Slim build, narrow frame.

OUTFIT: [YOUR OUTFIT HERE]

POSE: Standing, straight to camera, both hands loosely in pockets, shoulders
relaxed, looking directly at the lens.

SETTING: Cream panelled wall with simple wainscoting, herringbone parquet floor in
warm oak.

LIGHT: Soft even daylight from camera left, gentle shadow on the wall behind,
no harsh contrast.

CAMERA: Full body, head to shoes, nothing cropped. Shot on 85mm at f/4, eye level.

STYLE: Editorial menswear photography. Natural colour, realistic fabric drape,
visible texture in knitwear and cotton. No beauty retouching.

FORMAT: Vertical 2:3.

AVOID: Changing the face. Removing the glasses. Altering hair texture. Cartoon or
3D render look. Plastic skin. Extra fingers. Logos or brand names. Text or
watermarks. Harsh flash. Cropping the feet.
```

---

## OUTFIT LINES — ready to paste

Replace `[YOUR OUTFIT HERE]` with one of these. Written in the detail the model
needs: garment, colour, fabric, fit, and what is on the feet.

### Women — Khaki Shorts guide

| # | Outfit line |
|---|---|
| 01 | Tailored khaki cotton shorts, mid-thigh, with a cream ribbed knit tucked at the front only, and white leather trainers |
| 02 | Khaki shorts with a black fitted tank top and flat tan leather sandals |
| 03 | Khaki shorts with an oversized white cotton shirt worn open over a white vest, and brown loafers |
| 04 | Khaki shorts with a navy and white breton stripe long-sleeve top, sleeves rolled, and white canvas trainers |
| 05 | Khaki shorts with a cropped olive linen shirt tied at the waist and brown leather slides |

### Women — Leather Skirt guide

| # | Outfit line |
|---|---|
| 01 | Black leather midi skirt with a plain white cotton t-shirt tucked in, and white trainers |
| 02 | Black leather midi skirt with a cream chunky knit jumper worn loose over the top, and black ankle boots |
| 03 | Black leather mini skirt with an oversized grey sweatshirt and black leather loafers |

### Men — Tan Shorts guide

| # | Outfit line |
|---|---|
| 01 | Tan pleated cotton shorts with turn-up cuffs, a cream cricket knit with navy striped trim, white crew socks and black leather penny loafers |
| 02 | Tan pleated shorts with a plain white cotton t-shirt and white leather trainers, no socks visible |
| 03 | Tan pleated shorts with a pale blue oxford shirt, sleeves rolled to the elbow, and brown suede loafers |
| 04 | Tan pleated shorts with a navy polo shirt and white canvas trainers |

### Men — Brown Suit guide

| # | Outfit line |
|---|---|
| 01 | Chocolate brown wool suit, single breasted, with a crisp white shirt open at the collar and dark brown leather loafers |
| 02 | Brown suit trousers with the jacket carried over one arm, a pale blue shirt and white leather trainers |
| 03 | Brown suit worn with a fine-gauge cream knit instead of a shirt, and brown suede derbies |

---

## IMAGE SIZES THE SITE NEEDS

| Where | Size | Ratio |
|---|---|---|
| Hero | 1000 × 1500 | 2:3 |
| Guide card | 900 × 1200 | 3:4 |
| Audience panel | 900 × 1200 | 3:4 |
| Pinterest pin | 1000 × 1500 | 2:3 |
| Author portrait | 800 × 1000 | 4:5 |

Generate at 2:3 and crop down — it covers every slot except the author portrait.

---

## ONE RULE THAT MATTERS MORE THAN THE PROMPT

Keep the **setting and light identical** across a whole guide. Fifteen outfits in
fifteen different rooms looks like a Pinterest board. Fifteen outfits against the
same wall in the same light looks like a shoot — and that is what makes a new site
read as a real publication.

Change the room between guides if you like. Never inside one.
