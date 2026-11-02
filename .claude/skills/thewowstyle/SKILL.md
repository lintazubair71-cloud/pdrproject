---
name: thewowstyle
description: >-
  Content system for thewowstyle.co.uk (The Wow Style) — fashion and outfit-ideas
  styling guides for men and women. Use whenever researching, planning,
  structuring, or writing any article, pillar page, or sub-topic for The Wow
  Style: competitor research, keyword research, user-intent analysis, article
  structure, writing standards, internal linking, and the pre-submission audit.
  Triggers on "write an article for The Wow Style", "research/plan a styling
  guide", "pillar page", "how to style X", "outfit ideas", "sub-topic brief".
---

# The Wow Style — Content System

## Site Overview

- **Site:** thewowstyle.co.uk
- **Author / brand:** Aria James — Founder and Editor. Writes styling guides for men and women. Write in her first-person editorial voice where natural (this is a personal, expert-led brand — see Personal Voice & E-E-A-T below). (Do **not** invent extra credentials — years, client counts, awards. If Aria adds real ones later, use those.)
- **Niche:** Fashion and outfit ideas — image-led styling guides (how to style a garment, what to wear to an occasion, aesthetics, decade looks, accessories, seasonal, dress codes), for men and women.
- **Target audience:** US/UK, general fashion readers, beginner to intermediate. They arrive with one specific question ("how do I wear X?", "what do I wear to Y?") and want copy-able outfits, not theory.
- **Voice reference:** Who What Wear, Byrdie, InStyle (women/general); He Spoke Style, Real Men Real Style (men); The Trend Spotter (listicle format). Expert, specific, warm — never influencer-breathless. *(Not fixed in CLAUDE.md; adjust if Aria prefers others.)*
- **The 7 pillars (category concept `/fashion/`, but live URLs are one level deep):**

| # | Pillar | Pillar URL | Pillar head keyword | Format of its guides |
|---|---|---|---|---|
| 1 | How to Style | `/how-to-style/` | how to style clothes | "How to Style X: 15 Outfits" |
| 2 | Occasion Outfits | `/occasion-outfits/` | what to wear to any occasion | "X Outfits: 15 Ideas" |
| 3 | Fashion Aesthetics | `/aesthetics/` | fashion aesthetics explained | "X Fashion: 15 Looks to Try" |
| 4 | Fashion Accessories | `/accessories/` | fashion accessories guide | "X: 15 Ways to Wear" |
| 5 | Decade Fashion | `/decade-fashion/` | fashion through the decades | "X Fashion: N Outfits to Copy" |
| 6 | Seasonal Outfits | `/seasonal-outfits/` | seasonal outfit ideas | "X Outfits: N Ideas" |
| 7 | Dress Codes | `/dress-codes/` | dress codes explained | "X: What to Wear" |

### Source-of-truth files (read these; do not re-derive what they already decide)
- **`CLAUDE.md`** — project law: permalinks, title length, image rules, the ChatGPT image-prompt-pack standing instruction, affiliate disclosure placement.
- **`TheWowStyle_120_Article_Roadmap.xlsx`** — the canonical plan: Tab 2 PILLAR MAP (every pillar + its sub-topics), Tab 4 Article Details (title, primary + secondary keywords, audience, URL), Tab 5 Internal Linking (exact up/down/sideways/across links per article), Tab 6 Keyword Map (one keyword → one article). This file already eliminated topic overlap. **Do not re-invent the cluster, keyword ownership, or linking — read it.**
- `FEMALE-MODEL-PROMPT.md` / `MALE-MODEL-PROMPT.md` — model, poses, details, slot sizes for images.

> **First priority, above everything:** the reader's article, their intent, their need, their real queries, the solution to their problem. Every rule below exists to serve that. SEO/AEO/GEO/semantic are how the right reader finds the answer — never a reason to pad or distort it.

---

## OPERATING PRINCIPLES (apply to every step, every instruction)

These govern the whole workflow. If any later section seems to conflict, these win.

1. **Verify, never assume.** Every fact, URL, live-status, competitor, keyword, source, and claim is confirmed by actually checking — fetch the sitemap, fetch and read each competitor in full, open each source, search the SERP. Never act on memory, a snippet, or "probably". If something can't be verified, say so plainly and label it — do not fill the gap with a guess.
2. **Structure = user intent + what already ranks, fused — but intent wins.** Build every article's structure from both: what the reader needs answered (Step 3) and what Google already rewards for this query (Step 4 competitor structure). Where they agree, follow it; where a competitor pattern doesn't serve intent, drop it. The final structure must fulfil the searcher's intent completely — that is the test it has to pass.
3. **Write like a high-authority expert — personal voice.** The reader should feel within the first lines that a real expert (Aria James / The Wow Style) wrote this, not a generic content mill. First-hand styling judgment, specific calls, a consistent editorial voice — this is personal branding / E-E-A-T, and it is a ranking and trust asset. (Details in Personal Voice & E-E-A-T.)
4. **Every line earns engagement.** Every sentence gives the reader information or moves them forward; nothing is filler. The reader should want to keep reading to the end. Every H2 clearly and directly answers a real user query.
5. **Complete, not long.** Cover everything the reader needs — and stop. No extra length without a reason, no repeated information without a reason. Depth and completeness, never padding.
6. **Natural over forced — always.** Keywords (short/mid/long-tail), entities, LSI/semantic terms, and internal links go in only where they read naturally — the way a high-authority site drops a link mid-explanation or uses a term because the sentence needed it. If it has to be forced, it doesn't go in.
7. **Semantic + SEO + AEO + GEO on every article.** Topically complete (all the entities and sub-questions a knowledgeable reader expects), snippet-ready answers within the AEO character/word limits, and every factual claim backed by a strong, verified, authentic external source.
8. **Fill competitor gaps only where they genuinely help the reader.** A gap competitors missed is an opportunity *if* covering it serves this reader's intent and need. Don't add a section just because competitors lack it — add it because it helps.

---

## STEP 0: SITEMAP CHECK (mandatory before every task)

The site is early-stage: pillars and guides go live on a rolling schedule (roadmap Weeks 1–24). **Never assume a URL is live.**

Before writing, planning, or linking anything:
1. Fetch the live sitemap: `https://thewowstyle.co.uk/sitemap.xml` (or `/sitemap_index.xml`, or the WordPress/Yoast/RankMath sitemap). Record every live URL.
2. Reconcile against the **planned** URLs in `TheWowStyle_120_Article_Roadmap.xlsx` (Tab 4 Article Details). Remember the prefix difference: the roadmap lists `/fashion/how-to-style/<slug>/`; the **live site uses `/how-to-style/<slug>/`** (drop `/fashion/`). Pillar slugs: `how-to-style`, `occasion-outfits`, `aesthetics`, `accessories`, `decade-fashion`, `seasonal-outfits`, `dress-codes`.
3. Note any live page not in the roadmap, and any roadmap page not yet live.
4. **Never link to a URL that is not confirmed live on the sitemap.** A written-but-not-live target gets **bold placeholder text**, not a link.

If the sitemap cannot be fetched, say so plainly and do not guess live status — treat all targets as not-yet-live (bold placeholders) until verified.

---

## CONTENT ARCHITECTURE RULES

### Cluster logic
A cluster is one pillar page + its genuine child articles. A pillar is a real topic cluster, not a broad bucket.

**The test for every sub-topic:** "Does this article need the pillar topic as context to exist? Is it one specific angle of that pillar?" On The Wow Style this is already settled by the roadmap — **every one of the 120 articles belongs to exactly one pillar, chosen to not overlap any other.** So in practice:
- Do not move an article between pillars, or dump it under the nearest pillar, without re-running the overlap method in the roadmap's START HERE tab.
- There are very few true standalones here (unlike a science site). If you think something is a standalone, check the roadmap first — it probably already has a home.

### How overlap was eliminated (keep applying it)
From the roadmap's method — enforce it on any new topic:
1. **Reserved pillar head terms.** No sub-topic may target its pillar's head keyword (e.g. nothing under How to Style targets "how to style clothes"). The pillar covers the topic broadly; each sub-topic takes one specific garment/colour/piece.
2. **Content signature.** Normalise gender words, strip filler ("outfit", "ideas", "best", "style"), normalise plurals/apostrophes (`90s` = `90's`).
3. **Conflict rule.** Two articles whose signatures are a subset of each other, or ≥60% identical, conflict — only one survives.
4. **One keyword → one article** (roadmap Tab 6). Never let a second article chase a keyword another already owns.
5. **Watch the near-misses** that start with pillar language but belong elsewhere, e.g. `how to style summer dresses` is **Seasonal**, not How to Style.

---

## ARTICLE CREATION WORKFLOW

Follow in order. Do not skip a step.

### Step 1 — Sitemap verification
Run STEP 0. Confirm live URLs and record newly published pages.

### Step 2 — Cannibalization & overlap gate (kills the article before wasting research)
Decide whether this article has the right to exist on the site.

**A. Keyword-intent overlap.** Search Google: `site:thewowstyle.co.uk [target keyword]` and `site:thewowstyle.co.uk [primary intent phrase]`. For each result: does it already target the same primary keyword / answer the same core question / would Google see them as interchangeable? If yes to any → **STOP.** Report the conflict; recommend merge, sharply differentiate, or kill.

**B. Pillar coverage.** Fetch the pillar page. Read its section on this sub-topic. If the pillar already covers it in 200+ specific words → no room; STOP or trim the pillar first. If the pillar gives a 2–3 sentence teaser and defers → room exists; PROCEED.

**C. Sibling overlap.** List all live sibling articles in the same pillar (roadmap Tab 5 names the siblings). For each: does it already own an H2-level section this article needs? Shared long-tails that would split ranking? If overlap → write a **DO NOT COVER** list naming exactly what each sibling owns. The new article may not touch those angles.

**D. Output.** VERDICT: **GO / KILL / MERGE / DIFFERENTIATE.** If GO, carry the DO NOT COVER list into Step 5. If KILL/MERGE, explain and suggest the alternative.

### Step 3 — User intent analysis
Search the target keyword on Google and read the **actual SERP** before deciding intent.
- What format dominates the top 5 (outfit listicles, definitions, comparisons, shop pages, Pinterest)?
- What does the featured snippet answer, if any?
- What do the People Also Ask questions reveal readers still want?
- Is there a mismatch between the keyword phrasing and what Google rewards? Follow Google's signal, not the phrasing.

A question that appears only in competitors' FAQ sections is **secondary** intent. Primary intent is whatever every competitor leads with. Do not invert this.

**Intent types on The Wow Style:**
- **"How to style X"** → outfit-ideas listicle. N distinct, copy-able looks, head to toe, **shoes named in every look**. Minimal theory.
- **"What to wear to [occasion]"** → occasion listicle; lead with the appropriateness answer, then the looks.
- **"X outfit ideas / X outfits"** → listicle of looks.
- **"[Aesthetic] fashion / looks"** → short explainer of the aesthetic + looks that define it.
- **"[Decade] fashion"** → short, *accurate* decade explainer + outfits to copy.
- **"How to wear [accessory]"** → ways-to-wear listicle.
- **"What is [dress code] / [dress code]: what to wear"** → precise definition + what it does/doesn't allow + examples.
- **"X vs Y"** (e.g. smart casual vs business casual) → direct comparison + clear recommendation.

The reader who clicked the title has one question. Every section must serve it.

### Step 4 — Competitor research (mandatory, never optional)
Analyse the **top 10 genuinely competing** ranking pages for the target keyword. Fetch and read each in full — no snippets, no guessing. Exclude forums, social, irrelevant category pages, duplicates (unless they genuinely satisfy the intent). If a page can't be fetched, note it and move on. **Note the common reality in this niche:** many top results are thin, AI-spun or expired-domain spam — that is the opportunity (beat them on real photos, genuinely distinct looks, accuracy), but still read the strongest real competitors to find table stakes and gaps.

For each competitor page, extract:
- Full heading structure (H1 → H2 → H3, exact).
- Every subtopic the body actually covers (not just headings).
- FAQs (exact questions).
- Proof used (named sources, stats, historical/dress-code facts, brand/designer references, examples).
- Estimated word count and image count.
- Depth: Shallow / Moderate / Deep (one-line justification).
- Strengths: where it satisfies intent well.
- Weaknesses: surface-level, outdated, unclear, unsupported, or **factually wrong** (wrong decade, wrong dress-code rule, body-type/colour claims stated as settled).

**Competitor heading analysis (collectively):** repeated headings (table stakes), unique headings (differentiators), logical order, headings that target intent vs filler. Understand coverage and hierarchy — **do not copy headings.**

**Competitor content-structure analysis (each):** what it opens with, where it gives the quick answer, section order, how fast the key info is found, scannability, use of tables/lists/steps/examples/FAQs, buried answers, off-intent padding.

**Competitor fact & source audit (fashion version of the "external source audit"):**
- Which facts/claims do competitors assert — decade attributions, dress-code conventions, cultural/occasion rules, fabric/care, body-type/colour-season advice, trend/data claims?
- Where they cite a source, is it primary, credible, live, and does it actually support the claim?
- **Open the source yourself** and confirm it isn't misrepresented. Competitors routinely state as fact things that are contested (colour-season "rules", body-type "rules") or wrong (mislabelling a 2000s trend as 90s, confusing cocktail with semi-formal). **A correctly caught error that every competitor repeats is one of the strongest differentiators available.**
- Flag outdated, broken, weak, or commercially biased sources. Keep a separate list of verified sources worth using.

**Competitor comparison table:** URL | Word Count | Image Count | Depth | Key Strengths | Key Weaknesses | Unique Angles.

**Entity map (combined):** tag each entity `[MUST INCLUDE]` (3+ competitors) or `[DIFFERENTIATOR]` (1–2). Entities here = garments, colours, fabrics, fits, silhouettes, footwear, occasions, dress codes, aesthetics, decades, body types, designers/brands where relevant.

**Keyword & phrase mining (content-derived, categorise every term):** short-tail (1–2), mid-tail (3–4), long-tail (5+ / full questions), entities (tag MUST/DIFF), NLP/LSI terms competitors use naturally, PAA questions from the SERP, and **real user pain-point questions** from Reddit / forums / comments (what people actually ask: "does X make me look short?", "can I wear X to an interview?"). If forum data can't be retrieved, say so and label the pain points **inferred from competitor FAQ/headings** — never present inferred language as observed. Present as one table: Term | Category | Source | Placement suggestion (which H2/look).

**Gap analysis:** covered by all (table stakes) · by 1–2 (cover better) · by none but searchers want (biggest edge) · depth gaps (where they say "it depends" and stop) · format gaps (missing comparison table, step-by-step, outfit-by-outfit) · **accuracy gaps** (where competitors state something the facts don't support).

**Independent research (beyond competitors):** current trend data or authoritative references (2023–2026), emerging angles competitors missed, live PAA/related queries, widely cited facts no competitor mentioned. Present in a clearly labelled separate section.

**Duplication & relevance clean-up (before Step 5):** merge duplicate keywords, combine same-intent questions, remove repetitive section ideas, drop irrelevant entities/terms, confirm every proposed section connects to the primary keyword and intent, separate genuine gaps from things competitors already cover in different words.

### Step 5 — Article structure
Build from two inputs combined: **user intent** (Step 3) and **competitor structure** (Step 4). Satisfy intent first; follow competitor structure only where it serves intent; ignore it where it doesn't. Never copy it as a template.

Structure principles:
- Open with what the searcher wants — not history or a definition they didn't ask for.
- Order by urgency: what they need first → what helps next → what deepens last.
- Every H2 answers a specific question or pain point — if not, cut it.
- No H2 needs more than 3–4 H3s — if it does, split it.
- Carry over `[MUST HAVE]` / `[DIFFERENTIATOR]` tags.
- Enforce the DO NOT COVER list — no section may invade pillar or sibling territory.

**Article-type balance check (critical for this site):** the dominant content type must match the article type. On an outfit-ideas listicle, **the outfits are the body** — each look, its garments/colour/fabric/fit/shoes, why it works, and when to wear it carry the majority of the words. Theory, history, and any fact-correction stay a minority. Before writing, estimate the word split and confirm the article's own subject (the outfits) is the largest part. A clever fact-correction is a differentiator, not the article.

For each section specify: **Format** (paragraph / table / comparison / outfit list / step-by-step / quick list — whatever communicates fastest) · **Word range** (what the section needs, not a fixed target) · **AEO block** (mark 2–3 sections needing a 40–60-word snippet-ready direct answer at the top of the H2) · **GEO citations** (flag where a named source belongs — dress-code rule, historical fact, trend stat) · **Internal link placement** (anchor direction) · **Image placeholder** (every outfit look gets one — see Image Strategy).

**FAQ in structure:** 4–6 questions from the gap analysis + long-tails. Answers 2–3 sentences, self-contained, no cross-references.

**Structure output includes:** 2–3 title options (≤60 chars) · meta description (≤160 chars, includes primary keyword) · full H1→H2→H3 outline with format, word range, tags per section · section-by-section keyword/entity mapping · total estimated word count · top 3 differentiator sections · any competitor sections deliberately excluded and why.

### Step 6 — Write the article
Follow the structure precisely. Apply every writing standard below.

### Step 7 — Self-audit
Run the full checklist (end of this file) by **searching** the text, not by reading. Flag anything missed.

---

## WORD COUNT APPROACH

Content need sets length, not a preset number. **House anchor (CLAUDE.md): guides are image-led, 25–40 images, ~900–1,400 words** — the images carry much of the load, so text is tight and every line earns its place. Pillar pages run longer (comprehensive hub + links). Let competitor depth and entity coverage decide the exact figure. **Never add words to hit a number** — padding an outfit listicle with filler theory weakens it and breaks the article-type balance.

---

## ARTICLE STRUCTURE TEMPLATE

**H1:** primary keyword, natural phrasing.

**Quick Answer Box (AEO)** — under 60 words **and** under 320 characters (both), self-contained, snippet-ready. For a styling listicle: the one-line answer to "how do I wear X / what do I wear to Y" (the governing principle + the safest look).

**Key Takeaways** — 5 bullets, no overlap with the Quick Answer. Each summarises a **body** section. A takeaway must never preview a FAQ answer.

**Intro** — 2 paragraphs max, no filler. The reader clicked a specific question; within 2–3 sentences they must feel "this is exactly my answer." Front-load the core insight, then expand. No history, no "X is important because", no slow build.

**[Brand Authority Block — PILLAR PAGES ONLY]** — Aria James, Founder and Editor of The Wow Style, styling guides for men and women. **Credentials only, no "trust me" language.** Use only real attributes; do not fabricate years/clients. Omit entirely on sub-topics and standalones.

**[Quick Reference Table — only where data warrants]** — for dress-code comparisons, colour/season breakdowns, decade signatures, fit guides, or "X vs Y". Skip if the article has no comparative/structured data.

**The Outfits / Looks (the body — this is the article):** For listicles, each look is a compact unit:
- A short outfit line — **garment, colour, fabric, fit, and the shoes** (CLAUDE.md: every outfit names the shoes; shoes must be visible in-article).
- One or two lines on *why* it works and *when* to wear it (occasion, season, body-type note where genuinely helpful).
- Image placeholder for that look.
Keep looks genuinely distinct — no two that are the same outfit reworded. For explainer/comparison/dress-code articles, replace "looks" with the intent-matched H2s (definition → rules → examples → mistakes).

**FAQ** — 5–6 questions, 1–2 lines each, every answer genuinely **new** (not restating the body), self-contained (no "as above"), FAQPage JSON-LD ready.

**[Conclusion — intent-dependent]** — include for actionable articles (how-to, occasion, dress-code "what to wear") or where the reader needs a next step; 2–3 lines, reinforce the core takeaway + one concrete next action. Skip on pure explainers where Quick Answer + body already close the loop. Never repeat the intro, never summarise every section, never "In conclusion".

**[Affiliate Disclosure — where affiliate links appear]** — replaces the fitness site's medical disclaimer (fashion styling carries no injury risk). Per CLAUDE.md, the disclosure sits **above the first affiliate link**, not in the footer. 1 line, natural tone, e.g. "The Wow Style is reader-supported — some links earn us a commission at no cost to you." Omit if the article has no affiliate links.

**Author Attribution** — end of article (Aria James).

**Schema markup** — Article + FAQPage JSON-LD on every article; add **ItemList** for outfit/ways-to-wear listicles; ImageObject where images are primary. FAQPage answer text must match the rendered FAQ answers **word for word** — after any FAQ edit, re-sync the schema in the same pass.

**Meta title:** ≤60 characters. **Meta description:** ≤160 characters, includes primary keyword.

---

## WRITING STANDARDS

### Voice and tone — Personal Voice & E-E-A-T
Write like Who What Wear, Byrdie, or He Spoke Style — an editor speaking directly to the reader's specific question. Expertise shows through **specificity, precision, and genuinely good styling judgment**, never through claiming it. Demonstrate, don't announce.

**This is a personal, expert-led brand (Aria James / The Wow Style).** The reader should be able to tell a real expert wrote the piece — the way you can tell on a high-authority site — within the first few lines. How that shows up:
- **A clear point of view.** Make specific calls ("tuck the front hem only", "skip the belt here"), not hedged both-ways advice. A confident, defensible recommendation reads as expertise; "you could do X or Y or Z" reads as a content mill.
- **First-hand framing where natural.** First-person editorial voice is welcome ("I'd reach for a loafer over a trainer here, and here's why") — it signals real experience (the first E in E-E-A-T). Never fabricate a personal anecdote, but a genuine stylist's perspective is the voice to write in.
- **Specific over generic every time.** Name the exact garment, colour, fabric, fit, and shoe. "A rust-brown suede loafer" beats "nice shoes". Specificity *is* the authority signal.
- **Consistent editorial voice** across the whole piece and ideally the whole pillar — same confidence, same register, so the brand feels like one expert, not many templates.
- **Reader-first, not SEO-first on the surface.** It must read as if written purely to help the reader dress well; the optimisation is invisible underneath.

**Engagement — every line pulls the reader forward.** Every sentence delivers information or advances the look; cut anything that doesn't. Open each section on the answer, keep paragraphs tight, and make the reader want the next line. Every section connects to the next — the reader should feel pulled forward. The last 1–2 sentences of an H2 should raise the question the next section answers (content-driven, not a forced "Now let's look at…"). If two H2s sit next to each other and the reader feels a gap, the transition is broken. **A section must never end on an internal link** — that sends the reader away exactly when the next section needs them.

### Content rules
- User intent is the top priority — answer the question completely.
- Never open with a generic start. First lines speak to the reader's exact question.
- Stay on topic — cut anything that doesn't serve the core question.
- Do not inflate word count; if it's fully covered in 1,000 words, stop.
- No repeated information unless a genuinely different context needs it.
- Every H2 delivers new information and a clear answer.
- Short, clear paragraphs. Passive voice under 10% — prefer active, direct sentences.
- High readability throughout.

### Facts and claims handling (the fashion version)
Fashion is mostly styling judgment, which is the site's own expertise and does **not** need a citation ("pair it with white trainers for a casual weekend look" is judgment, not a sourced claim — do not bolt a fake source onto an opinion). But some fashion claims are **checkable facts and must be right, and sourced where appropriate**:
- **Decade / historical accuracy** — do not call a 2000s/Y2K trend "90s"; get era signatures right.
- **Dress-code conventions** — cocktail ≠ semi-formal ≠ black tie ≠ white tie; "smart casual", "business casual", "business formal" have real, distinct meanings. Precision here is the whole value of a dress-code article.
- **Cultural / religious / occasion appropriateness** — funeral, church, interview, wedding-guest, African attire, etc. Be accurate and respectful; state real conventions, not assumptions.
- **Fabric, care, and fit facts** — linen wrinkles, suede and rain, what a fabric does.
- **Any statistic, trend-data, or "studies show" claim** — needs a named, verified source.

Rules:
- Never invent statistics, dates, quotes, studies, or "expert says". Don't present unverified info as fact. Never state a contested styling "rule" as settled. Use "always/never/guaranteed" only with strong justification.
- **Scope-match:** a source's finding applies only to exactly what it covered. A convention in one culture/country is not universal; a "rule" for one body type is not for all; a UK dress-code norm may differ from a US one. Before attaching a source to a claim, state what it actually covers and confirm the claim doesn't travel past it.
- **Contested cues → body type & colour analysis:** "flattering for X body type", "best colours for your season/undertone" are contested and often pseudo-rules. Never state one side as settled. Give the specific, defensible version ("a higher waistline lengthens the leg line") or name the disagreement in one clause ("some stylists swear by seasonal colour analysis; others treat it as a starting point, not a rule"). Replace vague intensifiers ("slimming", "elongating") with the specific effect.
- **Absolutes** ("the only way to wear X", "you must never", "completely") claim more than styling earns — replace with what the choice actually does.
- Carry a source's own hedging into the article. Distinguish hypothetical examples from real evidence. If something can't be verified, say so instead of inventing it.

### AI writing pattern avoidance
Beyond the banned list: don't open every section the same way; don't overuse three-item lists or unnaturally symmetrical sentences; avoid mechanical transitions and repetitive section summaries; use natural sentence variation and contractions; vary paragraph structure (not every one claim-evidence-application); use topic-specific vocabulary (name the actual garment/colour/fabric/fit), not generic interchangeable language.

### Internal link sentence test
The surrounding sentence must stay useful even if the link is removed. If a sentence exists only to house a link, rewrite it to deliver value on its own.

### Keyword and entity placement
Place all keywords/entities from the analysis **naturally** — it must read correctly with SEO awareness removed. Priority: target keyword in intro + 1–2 H2s + conclusion; LSI/semantic terms across body; entities where contextually relevant. If a keyword can't fit naturally anywhere, don't use it.

### SEO / AEO / GEO / Semantic
- **SEO:** target keyword in H1, meta description, intro, and naturally through the body; variations in H2s where natural.
- **AEO:** `[AEO BLOCK]` sections open with a 40–60-word self-contained direct answer; Quick Answer box on every article, kept strictly within the limit (under 60 words **and** under 320 characters). Target the actual snippet format Google rewards for this query (paragraph / list / table).
- **GEO:** every claim that references a study, stat, historical fact, or dress-code authority includes a named, verified, linked source — generative engines extract cited content better.
- **Semantic:** cover the topic *completely* — all the entities, sub-questions and related concepts a knowledgeable reader (and the Step 4 entity map + PAA) expect — so the page reads as topically complete. "Semantically optimised" means depth and entity coverage, **not** repeating the keyword. Related terms appear because the subject genuinely calls for them.

---

## IMAGE & VISUAL STRATEGY

This is a visual, image-led site — images are central, not optional decoration. **This section works together with CLAUDE.md's image rules; CLAUDE.md wins on any conflict.**

- **Outfit / ways-to-wear / occasion / decade / aesthetic articles:** every look gets an image placeholder right after its outfit line. Specify what it shows and alt text with the keyword where natural (e.g. `alt="how to style khaki shorts women — linen shirt and tan sandals look"`). **Shoes must be visible** in the shot (CLAUDE.md).
- **Comparison / dress-code articles:** mark a placeholder for a comparison table or visual (e.g. a dress-code spectrum).
- **Pure explainers with nothing to show** (rare here): skip decorative placeholders.
- **Consistency (CLAUDE.md):** keep wall, floor, light direction and colour grade identical **within one guide**; one image style across a whole pillar; never reuse one photograph in two slots on the same page; audience panels frame from the knee up.
- **Image prompts enforce the outfit line.** Every outfit the text describes must appear in the prompt as an explicit garment/colour/fabric/fit + shoes; a different pose per image, rotated; one small imperfection per image; per-image framing (full body / three-quarter / waist-up / low angle / detail crop) and format (2:3 or 3:4); filenames matching the article slug. If a described look changes during the audit, update the matching image prompt in the same pass.
- **ChatGPT image-prompt pack (CLAUDE.md standing instruction):** when — **and only when** — asked, end the article with the full image-prompt pack (counts by type, variations per model, outfit line per image including shoes, poses, details, framing/format, exact filenames), pasteable one block at a time. Source of truth for models/poses/details/slots: `FEMALE-MODEL-PROMPT.md`, `MALE-MODEL-PROMPT.md`. Do not append the pack unprompted.

---

## EXTERNAL CITATION RULES

Fashion needs far fewer citations than a science site — **cite facts, not opinions.** Where a claim is factual (decade/history, dress-code convention, cultural attire, fabric science, a statistic or trend figure), it must carry a named, verified, working link.

- **Source quality (fashion-appropriate):** recognised fashion/history/etiquette authorities and primary sources — e.g. Vogue / Business of Fashion / established fashion desks for trends; Debrett's or equivalent for formal dress-code etiquette; museum, brand-heritage, or historical references for decade/era facts; official bodies for cultural/traditional attire; textile/fabric authorities for fabric claims; reputable data sources for any statistic. For the rare health-adjacent claim (e.g. UV and sunglasses), use a medical authority.
- **Recency:** use current references; check for newer data before citing older.
- **Placement:** the citation appears next to the claim it supports.
- **Link only what you opened.** If the canonical source can't be fetched, link the record you did open and note which. A source verifiable nowhere is dropped (and the drop recorded), never published with a guessed link.
- **Primary over secondary.** Prefer the original/authority over a competitor's interpretation.
- **Accuracy of representation.** Don't exaggerate or decontextualise; carry the source's hedging; keep the citation close to the claim.
- **Don't cite common knowledge / styling judgment.** Obvious statements and the site's own outfit recommendations don't need a source.
- **No competitor links — ever.** Never link to a direct competitor styling site.

---

## STYLING & FACT CLAIM VERIFICATION (mandatory for any article making factual claims)

The fitness site's hardest failures came from confidently-written-but-unchecked technique cues. The Wow Style equivalent: confidently-written-but-wrong **fashion facts** — a trend pinned to the wrong decade, a dress-code rule stated loosely, a body-type/colour "rule" stated as settled, a cultural attire claim that's inaccurate or disrespectful. Closing that gap is not optional.

Before submitting any article that makes factual claims (decade, dress-code, cultural/occasion, fabric, statistic, or body-type/colour), list every such claim and label each:

- **VERIFIED** — an authoritative source states it. Keep as written; record the source.
- **CONTESTED** — credible sources disagree (most body-type and colour-season "rules" land here). Don't state one side as settled. Rewrite to the specific defensible version, or name the disagreement in one clause. Record both sides.
- **INFERENCE / JUDGMENT** — your own styling reasoning with no source behind it. Allowed, and it's the heart of the site — but don't word it as an established finding and never attach a citation to it. ("This elongates the leg line" as a visual effect is fine; "studies prove this is slimming" is not.)

Particular traps (each already a known failure mode):
- Attaching a citation to something the source never covered (scope-match).
- Pairing a sourced claim and an unsourced one in one sentence so the citation seems to cover both.
- Decade mislabelling (2000s/Y2K called "90s", etc.).
- Blurring dress codes (cocktail/semi-formal/black-tie treated as interchangeable).
- Universalising a norm (one culture's or country's convention stated as global).
- Stating a contested body-type/colour rule as fact.
- A styling claim in the body that contradicts a fact cited elsewhere in the same article — check every cue against the article's own citations, not just outside sources.

Record the full pass in the deliverables: every claim, its label, its source, and what changed. "All facts verified" with no list is not a verification pass.

---

## INTERNAL LINKING RULES

The exact links are already specified per article in **roadmap Tab 5 (Internal Linking)** — read it; don't invent links. The rules it encodes:
- **UP:** every sub-topic links to its pillar **once**, inside the first 150 words, anchor = the pillar head keyword (one link, not three).
- **DOWN:** every pillar links to **all** its live sub-topics (a sub-topic the pillar doesn't link to is an orphan).
- **SIDEWAYS:** every sub-topic links to 2–3 siblings in the **same** pillar, on a genuine shared term (roadmap names the siblings and the shared term). Where two same-pillar articles share no term, link via the pillar instead — don't force one.
- **ACROSS:** cross-pillar link only where a shared term makes it natural (roadmap flags which ~1/3 of articles have one). If it says "do not force one", add none — a forced cross-link is worse than none.
- **CATEGORY:** homepage links to all 7 pillars; all 7 link back.

General: **max 3–4 internal links per article** (more only if every one is natural); natural mid-sentence anchor text only; never "click here / read more"; if a link doesn't fit naturally, skip it; **never link to a page not yet live — use bold placeholder text** until the sitemap confirms it.

---

## SUB-TOPIC BRIEF FORMAT

When planning a new sub-topic, always provide:
- Pillar page URL it belongs to (live `/pillar/` slug, from the roadmap).
- Unique angle for this article only.
- DO NOT COVER list (what the pillar and sibling articles already own).
- Confirmed internal URLs to link (verified live against the sitemap).
- Bold placeholder text for any target not yet live.

---

## BANNED PHRASES

Never use in article content (generic AI tells + fashion clichés):

"In this article we will" · "Looking for X?" · "It depends" without specifics · "Many people struggle" · "Without further ado" · "We hope you found this helpful" · "There are many types of X" · "Great question" · "Absolutely" · "Certainly" · "As an AI" · "Straightforward" · "Dive into" / "Let's dive in" · "Game changer" · "It's worth noting" · "It's important to note" · "significantly" · "transform" · "In today's world" · "Whether you're a beginner or advanced" · "In conclusion" · "very" · "really" · "actually" · "basically" · "essentially" · "incredibly" · "Same X. Same Y." fragmented patterns

Fashion-specific clichés to avoid: "effortlessly chic" · "effortlessly cool" · "elevate your look/wardrobe" · "fashion-forward" · "turn heads" · "on-trend" · "must-have" · "slay" · "fashionista" · "look no further" · "the perfect [X]" · "timeless classic" (as filler) · "versatile piece" (as filler) · "pop of colour" (as filler) · "wardrobe essential/staple" (as filler) · "flatter your figure" (vague — say the specific effect) · "take your outfit to the next level" · "ooze/exude [confidence/elegance]".

*(Legitimate garment/colour/fabric/fit vocabulary is not banned — the ban targets empty filler and hype, not real description.)*

**Check by searching** the finished text for each term, headings included. Reading the draft and judging it clean does not find them — a search does.

---

## POST-WRITING DELIVERABLES

After every article, include:

1. **Keyword & Entity Placement Report** — Keyword/Entity | Section | Placed Natural (Y/N).
2. **Unplaced Keywords & Entities** — any that couldn't be placed naturally, with reason.
3. **Internal Links Used** — Anchor Text | URL | Section (all verified live).
4. **External Links Used** — Source | URL | Section | Why Cited | What the source actually covers.
5. **Styling & Fact Claim Verification Log** — Claim | Label (VERIFIED / CONTESTED / INFERENCE) | Source | Action taken.
6. **Sources Dropped** — any considered and dropped, with reason (unverifiable, superseded, misrepresented by competitors).
7. **Missed Instructions Check** — review all instructions; flag anything missed or compromised. State "All instructions followed" only after running every mechanical check below.

---

## SELF-AUDIT CHECKLIST (run before every submission)

Run mechanical checks by **searching** the text, not by reading it.

- [ ] No AI wording or banned phrases — searched term by term, headings included
- [ ] No fluffy / hype language
- [ ] No repeated information across sections
- [ ] Quick Answer under 60 words **and** under 320 characters
- [ ] Key Takeaways don't overlap the Quick Answer; none previews a FAQ answer
- [ ] FAQs are genuinely new vs the body — verified by searching the body for each FAQ's key terms
- [ ] FAQPage JSON-LD answer text matches rendered FAQ answers word for word
- [ ] All keywords placed naturally — none forced
- [ ] Internal links natural, no generic anchors; **all verified live on the sitemap**; non-live targets are bold placeholders
- [ ] No section ends on an internal link; max 3–4 internal links (unless all natural)
- [ ] AEO Quick Answer box present; 2–3 AEO blocks open with a 40–60-word direct answer
- [ ] GEO — every factual claim has a named, verified, linked source; every external link was actually opened
- [ ] Every H2 answers one clear question; flow never breaks between sections (read transitions in sequence)
- [ ] No pillar-content overlap; DO NOT COVER list enforced; cannibalization gate passed
- [ ] Brand Authority Block on pillar pages only, credentials only, no fabricated numbers
- [ ] Affiliate disclosure above the first affiliate link (not footer), where links exist
- [ ] Passive voice under 10%; no correlation stated as causation
- [ ] **Styling & Fact Claim Verification pass complete** — every factual claim labelled VERIFIED / CONTESTED / INFERENCE, log included
- [ ] Scope-match confirmed on every citation — no convention/rule applied beyond what the source covers
- [ ] No contested body-type/colour claim stated as settled; no absolute ("the only way", "never", "completely") unearned
- [ ] No decade/dress-code/cultural fact wrong; no body claim contradicts a fact cited elsewhere
- [ ] **Article-type balance correct — the outfits/looks are the largest part of the body**, not theory or fact-corrections
- [ ] Image placeholders present where warranted; every outfit names the shoes and shoes are visible; prompts match final outfit lines (including any changed in the audit); one image style across the pillar
- [ ] No identical sentence structure opening every section; no look is another look reworded
- [ ] Internal-link sentences useful even without the link
- [ ] External sources primary (not secondary), conclusions not exaggerated, source hedging preserved
- [ ] Hypothetical examples distinguished from real evidence
- [ ] Keyword & Entity Placement Report + full post-writing deliverables included (verification log + dropped sources)
- [ ] Titles ≤60 chars; meta description ≤160 chars; H1 matches title intent
