# SEO Analysis & Fix Plan — Calorie Burn Calculator
**Page:** https://exercisemenu.com/calorie-burn-calculator/
**Data source:** Google Search Console export — last 28 days (US, Web), pulled 2026-11-01
**Prepared:** 2026-11-01

> ⚠️ **Access note:** The live page (`exercisemenu.com`) and competitor sites could not be
> fetched directly — this cloud session's network blocks those hosts, and the page's source
> code is **not** in this repository (it is empty). So this report is built from (a) your GSC
> export, (b) web-search competitor intelligence, and (c) calorie-calculator best practice.
> To do precise surgical edits on the live page and to audit/fix the tool itself, I need either
> the domain whitelisted in the session network settings, or the page's HTML/source (or WP access).

---

## 1. The headline problem (read this first)

| Metric (28 days, US) | Value | What it means |
|---|---|---|
| Clicks | **1** | Almost nobody is clicking through |
| Impressions | **232** | The page *is* being shown in search |
| CTR | **0.43%** | Catastrophically low — expected ~15–30% at this position |
| Avg position | **6.56** | Decent — the page ranks, often page 1 |

**You do not have a ranking problem first — you have a CLICK problem, plus a slow ranking decline.**
The page shows up at **position 1–3 for many real queries and still gets zero clicks:**

- `how many calories did i burn` → pos **1.67** (6 impressions, 0 clicks)
- `how many calories burned` → pos **3.25** (0 clicks)
- `calories burned` → pos **3.33** (0 clicks)
- `calorie burn calculator` → pos **3.0** (0 clicks)
- `how many calories do i burn` → pos **1.0** (0 clicks)

When a page sits at position 1–3 and earns ~0% CTR, Google's algorithm reads that as *"users don't
want this result"* and **demotes it over time.** That is exactly what your Chart.csv shows:

```
Oct 03–08:  position ~3–7   (good)
Oct 20–26:  position ~3–7   (holding)
Oct 29:     position 12.1   (slipping)
Oct 30:     position 21.0   (dropped off page 1)
```

So the drop you noticed is real, and the low CTR is almost certainly **causing** it. Fixing the
title/snippet and content depth is the priority.

---

## 2. Why the CTR is near zero (root causes)

1. **Title & meta description are not compelling / not keyword-aligned.** This is the #1 lever.
   (I can't confirm the current title without page access, but a 0.43% CTR at position 3 is a
   near-certain title/snippet failure.)
2. **The page reads like a chat transcript, not an SEO page.** Look at the queries it ranks for:
   `160 lbs`, `i weigh 130`, `53 kg`, `6'5 250`, `age 25`, `what about a light jog`, `what if i run?`,
   `yes`, `with the steps`, `treadmill`, `resistance bands`, `incline 8`, `gentle recovery`.
   These are **conversational fragments** — your tool is an AI/chat-style calculator and Google is
   indexing the conversation text. That text has **no click value** and dilutes topical focus.
   Google can't show a clean, trustworthy snippet, so users skip it.
3. **Thin supporting content.** Competitors rank with a full MET activity table, a formula
   explanation, examples, and an FAQ. If your page is "just the tool," Google has little to anchor a
   rich, clickable result on.
4. **No structured data** (FAQPage / WebApplication / HowTo) → no rich snippets → plain, low-CTR
   listing.

---

## 3. Keyword gap analysis (from YOUR Search Console data)

The page already **ranks** for these — it just needs on-page content/UI to convert impressions into
clicks and to climb. These are grouped by intent. **Everything below is a keyword you are already
visible for**, so it's low-effort, high-probability.

### A. Core / head terms (protect & win these — highest value)
| Query | Pos | Action |
|---|---|---|
| how many calories did i burn | 1.67 | Make this the H1 angle / featured answer |
| how many calories burned | 3.25 | Title + intro |
| calories burned | 3.33 | Title keyword |
| calorie burn calculator / calculator | 3.0 | Primary keyword (already in URL) |
| how many calories burned calculator | 17 | Add exact phrase in H2 |
| exercise calorie calculator | 42 | Add "exercise" synonym block |
| calorie calculator with exercise | 35 | H2 / intro |
| workout calorie burn / workout calculator | 22–25 | Synonym coverage |

### B. Activity-specific calculators (LOW volume, easy wins — exactly what you asked for)
These are gold. Each one can be won by a **single row in a MET activity table** + a short anchor.
| Query | Pos |
|---|---|
| how many calories does ab workout burn | 1.0 |
| how many calories do crunches burn | 5.0 |
| epoc calculator | 6.67 |
| afterburn effect calculator | 7.5 |
| crossfit calories burned calculator | 9.33 |
| tai chi walking calories burned calculator | 9.5 |
| gazelle calories burned calculator | 10.0 |
| leg press calories burned calculator | 10.5 |
| leg extension calories burned | 10.33 |
| how many calories does hip thrusts burn | 11.0 |
| standing calorie(s) burned calculator | 11–28 |
| heart rate to calories burned calculator | 18–26 |
| hiit training calories burned calculator | 28 |
| how many calories does a 180 lb man burn in a day | 11 |

### C. "How long to burn X calories" (reverse calculator — a missing feature)
| Query | Pos |
|---|---|
| how long does it take to burn 70 calories | 1.0 |
| how long to burn 150 calories | 2.0 |
| how long does it take to burn 350 calories | 7.0 |
| how long does it take to burn 130 / 250 calories | 10.0 |
| jogging for 5 minutes burns how many calories | 8.0 |
| running for 20 / 30 minutes calories | 5.0 |
➡ **Add a "How long to burn ___ calories" mode / reference table.** You rank for these with no
dedicated feature — adding one is a clear win.

### D. Homework / quiz questions (big impression driver, low commercial value)
These drove the most impressions of any single queries (10 + 12 impressions):
- *"about how long would a 150-pound person have to jog ... bagel ..."* (12 imp, pos 10.4)
- *"what activity burns about 405 calories per hour? bowling/soccer/sleeping/reading"* (7 imp)
- *"in an hour, a jogger burns about 4 calories per pound ... 151 pounds ..."* (12 imp)

Students are finding you for textbook questions. Low money value, but a **"Common calorie-burn
questions & examples"** FAQ block captures these impressions for free and adds the exact long-tail
text Google is matching.

---

## 4. Competitor landscape (what the ranking pages have that you likely don't)

From search intelligence, the pages that win "calories burned calculator" share a repeatable recipe:

| Element | Marathon Handbook | Runbundle | Omni | Inch Calc | **You (gap?)** |
|---|---|---|---|---|---|
| Large MET activity database | 800+ activities | 1,300+ | custom MET input | yes | **likely missing/thin** |
| Formula shown (ACSM: MET×3.5×kg/200) | ✅ | ✅ | ✅ | ✅ | **add it** |
| Cites Compendium of Physical Activities | ✅ | ✅ | — | — | **add — E-E-A-T** |
| FAQ section | ✅ | — | ✅ | ✅ | **add + schema** |
| "Net vs gross" calories option | — | — | ✅ (MET−1) | — | nice-to-have |
| Per-activity & per-duration examples | ✅ | ✅ | ✅ | ✅ | **add table** |
| Clean, keyword-rich title/snippet | ✅ | ✅ | ✅ | ✅ | **fix first** |

**Your structural gaps, in priority order:**
1. Compelling title + meta description (CTR).
2. Comprehensive MET activity table (captures all the activity long-tails in §3B).
3. Formula + methodology + credible source citation (E-E-A-T, helps post-"helpful content" ranking).
4. FAQ with FAQPage schema (captures §3D, enables rich results).
5. A "how long to burn X calories" reference/mode (captures §3C).
6. Clean up / de-index the conversational chat text if it's being crawled (topical focus).

---

## 5. Meta title suggestions (pick one — all ≤ ~60 chars)

Primary recommendation (balances head term + CTR hook):
1. **`Calorie Burn Calculator — How Many Calories Did I Burn?`**
2. `Calories Burned Calculator | By Exercise, Activity & Time`
3. `Calorie Burn Calculator: 300+ Exercises & Activities`
4. `How Many Calories Did I Burn? Free Calorie Burn Calculator`
5. `Calories Burned Calculator — Running, Walking, Gym & More`

**Meta description (≤ ~155 chars):**
> `Instantly see how many calories you burned. Free calorie burn calculator for 300+ exercises — running, walking, HIIT, strength, CrossFit & more. Enter weight & time.`

Alt description (question-led, good for CTR):
> `How many calories did you burn? Calculate calories burned by activity, body weight and duration — plus how long it takes to burn 100, 300 or 500 calories.`

**H1 suggestion:** `Calorie Burn Calculator` with a sub-line / lead paragraph answering
*"How many calories did I burn?"* (matches your #1-ranked query).

---

## 6. Prioritised action plan

**🔴 Do this week (CTR rescue — stops the ranking slide):**
1. Rewrite the **title tag** and **meta description** (§5).
2. Add a real **H1 + 80–120 word intro** that uses: *calories burned calculator, how many calories
   did I burn, by exercise/activity, body weight, duration.*
3. Make sure the page returns a **clean, static, crawlable** version of the core content (not only
   chat output). If the tool injects conversation text into the HTML, stop that text from being
   indexed (render it client-side, or mark it so it isn't the primary content).

**🟠 Next (depth — wins the long-tails):**
4. Add the **MET activity table** (ready-made in `calorie-burn-calculator-content-block.html`).
5. Add the **FAQ + FAQPage schema** (same file).
6. Add a **"How long to burn X calories"** reference table / calculator mode.
7. Add **WebApplication + HowTo schema** for the tool.

**🟡 Ongoing (authority & monitoring):**
8. Add a short **methodology** note citing the *2011 Compendium of Physical Activities* and the
   **ACSM** formula; add an author / reviewer line (E-E-A-T).
9. Internally link from related exercisemenu.com pages with anchor text like *"calories burned
   calculator"* and *"how many calories did I burn."*
10. Re-pull GSC in 3–4 weeks. Watch: avg position recovering toward 3–5, CTR rising above ~2–3%,
    and new activity long-tails entering top 10.

---

## 7. Tool issues to check (needs page/code access to confirm & fix)

I could not see the tool, but given the query signatures, check these:
- **Conversational text being indexed** — biggest SEO risk (see §2.2 / §6.3).
- **No static fallback content** — if the calculator is JS-only with an empty HTML shell, Google
  sees a thin page.
- **Mobile beats desktop** in your data (mobile pos 4.45 vs desktop 9.26) → check the **desktop
  layout/content** isn't weaker or pushing content below the fold.
- **URL parameters / chat states** possibly creating indexable junk variants (check Coverage report).
- Confirm **one canonical URL**, correct `<title>`, and that schema validates.

➡ Share the page HTML or whitelist the domain and I'll (a) apply exact title/meta/content edits and
(b) do a full functional + SEO audit of the tool and fix bugs directly.
