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

## MAKING IT NOT LOOK AI-GENERATED

The single biggest giveaway is not the face — it is **fifteen photographs of the
same person standing in exactly the same position**. No real shoot produces that.

So vary three things on every image. Keep everything else locked.

### 1. Rotate the pose

Never use the same pose twice in a row. Work down this list and start again:

| # | Pose line to paste |
|---|---|
| 01 | Standing straight to camera, weight on one leg, arms relaxed at her sides |
| 02 | Standing three-quarter turn to camera left, looking back over the shoulder at the lens |
| 03 | Mid-step walking toward the camera, one arm swinging naturally, looking just past the lens |
| 04 | Standing with one hand in a pocket, the other adjusting a sleeve or collar |
| 05 | Leaning lightly against the wall, shoulders square, ankles crossed |
| 06 | Standing with arms loosely folded, chin slightly down, looking at the lens |
| 07 | Turning away from camera, caught mid-turn, head coming back toward the lens |
| 08 | Seated on a plain wooden stool, one foot on the rung, hands resting on the knee |
| 09 | Standing in profile, head turned to the camera, hands clasped in front |
| 10 | Standing with one hand lifting the hem or holding a bag strap, looking slightly off-camera |

### 2. Change the framing

Do not shoot every look head-to-toe. Mix these in:

| Framing line | Use it for |
|---|---|
| Full body, head to shoes, nothing cropped | the main look shot |
| Three-quarter crop, mid-thigh up | when the top half is the point |
| Waist-up, closer | collars, necklines, layering |
| Low angle from just below waist height, full body | makes trousers and shoes look longer |
| Detail crop — hands, hem, shoe and ankle only | breaks up a long gallery, very pinnable |

A guide of fifteen identical full-body shots reads as AI. Eleven full-body, two
waist-up and two detail crops reads as a shoot.

### 3. Add one imperfection

Pick one per image and write it into the prompt:

- *a soft crease at the elbow and across the lap where the fabric has been sitting*
- *one sleeve pushed slightly higher than the other*
- *a few strands of hair out of place across the cheek*
- *the shirt hem sitting slightly uneven*
- *a shoe turned very slightly inward, natural stance*
- *fabric caught mid-movement, a little lift at the hem*

Perfect symmetry and flawless fabric is what makes an image feel generated. One
small asymmetry fixes most of it.

### Keep these locked — never vary them

The face, the hair, the glasses, the wall, the floor, the light direction and the
colour grade. Vary the person and the room and you no longer have a brand; you
have a stock library.

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

POSE: [ROTATE — pick a different one from the pose table each time]

DETAIL: [ONE imperfection from the list — e.g. a soft crease at the elbow]

SETTING: Plain warm-grey studio wall, pale oak floor.

LIGHT: Large soft window light from camera left, gentle falloff to the right,
soft shadow under the feet. Daylight, no flash.

CAMERA: [ROTATE framing — full body / three-quarter / waist-up / low angle / detail crop]
Shot on 85mm at f/4.

STYLE: Editorial fashion photography. Natural colour, no heavy grading, no beauty
retouching. Garments must drape realistically with visible fabric weight and
natural creasing.

FORMAT: Vertical 2:3.

AVOID: Changing the face. Altering hair length or colour. Cartoon or 3D render
look. Plastic skin. Extra fingers. Logos or brand names. Text or watermarks.
Harsh flash. Heavy makeup. The same pose as the previous image. Perfect symmetry.
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

POSE: [ROTATE — pick a different one from the pose table each time]

DETAIL: [ONE imperfection from the list — e.g. one sleeve pushed higher than the other]

SETTING: Cream panelled wall with simple wainscoting, herringbone parquet floor in
warm oak.

LIGHT: Soft even daylight from camera left, gentle shadow on the wall behind,
no harsh contrast.

CAMERA: [ROTATE framing — full body / three-quarter / waist-up / low angle / detail crop]
Shot on 85mm at f/4.

STYLE: Editorial menswear photography. Natural colour, realistic fabric drape,
visible texture in knitwear and cotton. No beauty retouching.

FORMAT: Vertical 2:3.

AVOID: Changing the face. Removing the glasses. Altering hair texture. Cartoon or
3D render look. Plastic skin. Extra fingers. Logos or brand names. Text or
watermarks. Harsh flash. The same pose as the previous image. Perfect symmetry.
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

---

## CHANGING THE OUTFIT FOR A SPECIFIC SLOT ON THE SITE

Each slot crops differently and some have text sitting over the picture, so the
composition has to suit the slot — not just the outfit.

### What each slot needs

| Slot | File size | Crop | What the composition must allow |
|---|---|---|---|
| **Hero** | 1000 × 1500 (2:3) | shown nearly whole | Clean wall behind. Subject slightly off-centre so the frame does not feel posed. |
| **Guide card** | 900 × 1200 (3:4) | top-anchored | Head must sit in the upper third. Feet may be cut. |
| **Audience panel** | 900 × 1200 (3:4) | top-anchored, **caption covers the bottom 25%** | Nothing important in the lower quarter. Face high in frame. Shoes will be hidden. |
| **Pinterest pin** | 1000 × 1500 (2:3) | shown whole | Leave headroom at the top for a text overlay. |
| **In-article look** | 1000 × 1500 (2:3) | shown whole | Full body, shoes visible — the shoes are half the styling advice. |

The one that catches people out is the **audience panel**: the caption sits over the
bottom of the picture, so a full-length shot loses its shoes and half the trousers.
Frame that one from the knee up.

### The prompt

```
Keep the exact same face, hair, glasses and body from the attached photo.
Change only the clothing.

SUBJECT: Man in his mid twenties, mixed race, medium-brown skin with a warm
undertone and natural texture. Dark brown tightly curled hair, short at the sides,
a few inches of loose curls on top. Thin round pale-gold wire-frame glasses. Fine
moustache and a small neat chin beard. Small stud earring. Calm neutral expression.
Slim build, narrow frame.

OUTFIT: [PICK A LINE FROM THE TABLE BELOW]

POSE: [ROTATE from the pose table]

DETAIL: [ONE imperfection from the list]

SETTING: Cream panelled wall with simple wainscoting, herringbone parquet floor
in warm oak.

LIGHT: Soft even daylight from camera left, gentle shadow on the wall behind,
no harsh contrast.

CAMERA: [SEE SLOT TABLE — full body / knee up / waist up]
Shot on 85mm at f/4, eye level.

STYLE: Editorial menswear photography. Natural colour, realistic fabric drape,
visible texture in knitwear and cotton. No beauty retouching.

FORMAT: [2:3 for hero, pin and in-article · 3:4 for cards and panels]

AVOID: Changing the face. Removing the glasses. Altering hair texture. Cartoon or
3D render look. Plastic skin. Extra fingers. Logos or brand names. Text or
watermarks. Harsh flash. The same pose as the previous image. Perfect symmetry.
```

### Outfit lines for the men's guides

Written in the detail the model needs — garment, colour, fabric, fit, and shoes.

| Guide | Outfit line |
|---|---|
| Brown Suit Men | Chocolate brown wool suit, single breasted, with a crisp white shirt open at the collar and dark brown leather loafers |
| Beige Pants Men | Beige cotton chinos, straight leg, with a white crew-neck t-shirt and white leather trainers |
| Grey Pants Men | Mid-grey wool trousers, pleated, with a navy fine-gauge knit and black leather derbies |
| White Pants for Men | White cotton trousers, straight leg, with a pale blue oxford shirt, sleeves rolled, and tan suede loafers |
| Green Pants Outfit Men | Olive green cotton trousers, relaxed fit, with a cream knit polo and white trainers |
| Purple Jeans Men | Deep purple straight-leg jeans with a plain black t-shirt and black leather boots |
| Men Stacked Jeans | Dark indigo jeans stacked over the ankle, with an oversized grey sweatshirt and white high-top trainers |
| Leather Pants Men | Black leather trousers, slim straight, with a white ribbed vest and black Chelsea boots |
| Grey Sweatpants Men | Heather grey sweatpants, cuffed, with a cream hoodie and white running trainers |
| White Suits for Men | Off-white linen suit, unlined, with a plain white t-shirt underneath and tan leather sandals |
| Pink Button Up Shirt Men | Pale pink cotton shirt, sleeves rolled to the elbow, with cream chinos and brown suede loafers |
| Casual Dress for Men | Navy knitted polo with beige pleated trousers and brown leather loafers |
| Chunky Shoes Men | Chunky-soled black leather trainers with straight-leg black jeans and a grey crew-neck knit |

### Worked example — Men's audience panel

Note the framing: knee up, because the caption will cover the bottom of the frame.

```
Keep the exact same face, hair, glasses and body from the attached photo.
Change only the clothing.

SUBJECT: [paste the subject block above]

OUTFIT: Beige cotton chinos, straight leg, with a white crew-neck t-shirt and a
navy overshirt worn open.

POSE: Standing three-quarter turn to camera left, one hand in a pocket, looking
back toward the lens.

DETAIL: The overshirt collar sitting slightly uneven.

SETTING: Cream panelled wall with simple wainscoting.

LIGHT: Soft even daylight from camera left, gentle shadow on the wall behind.

CAMERA: Framed from the knee up, subject slightly right of centre, headroom above.
Shot on 85mm at f/4, eye level.

STYLE: Editorial menswear photography. Natural colour, realistic fabric drape.
No beauty retouching.

FORMAT: Vertical 3:4.

AVOID: Changing the face. Removing the glasses. Placing anything important in the
lower quarter of the frame. Cartoon look. Plastic skin. Extra fingers. Logos.
Text or watermarks.
```

### Saving it

| Slot | Filename |
|---|---|
| Men's audience panel | `images/audience-men.jpg` |
| Tan shorts card | `images/khaki-shorts-men.jpg` |
| Any new men's guide card | `images/<guide-slug>-men.jpg` |

Use the same slug as the article URL. The site loads these paths already, so a
correctly named file appears without touching the code.
