---
name: listing-optimization-checklist
description: A structured pre-launch QA workflow for e-commerce product listings on Amazon and TikTok Shop. This skill should be used when a seller needs to review or rewrite a product title, five bullet points, backend search terms, product description, or listing images before publishing, or when an audit of an existing listing is requested. It provides fact-check-first discipline, platform-specific rules, and copy templates to avoid unsubstantiated claims.
description_zh: "电商 Listing 上架前自检流程：标题、五点、图片、搜索词、描述的逐项核对与改写"
description_en: "Pre-launch listing QA workflow: title, bullets, images, search terms, and description"
version: 1.0.0
agent_created: true
display_name: "Listing 优化清单"
display_name_en: "Listing Optimization Checklist"
visibility: "public"
tags:
  - ecommerce
  - amazon
  - tiktok-shop
  - listing
  - copywriting
  - qa
---

# Listing Optimization Checklist

## Purpose

Provide a repeatable, fact-check-first workflow for auditing and rewriting e-commerce product listings. The workflow is designed for Amazon and TikTok Shop but applies to any catalog-based marketplace. Every rule in this skill is verifiable — no vague "best practices."

Core principle: **complete the product fact sheet before writing any copy.** Every number in the final listing must trace back to the spec sheet.

## When to Use

- User asks to review, audit, or improve a product listing
- User asks to rewrite a title, five bullet points, or product description
- User asks which images to use or how to order gallery images
- User wants backend search terms optimized
- User wants a pre-launch checklist before publishing a listing
- User asks about differences between Amazon and TikTok Shop listing rules

## Workflow

### Step 1 — Gather facts

Load `assets/fact-sheet-template.md` and have the user fill it in for the target SKU. Do not proceed to copywriting until the fact sheet is complete. Extract these inputs:

- Full specs (model, dimensions, RMS and Peak power separated, materials, voltage, certifications)
- Three concrete use scenarios (who, where, doing what)
- Five real buyer pain points from reviews, questions, or support logs
- Three competitor listings (title, bullets, main image)
- A "do not claim" list: unsubstantiated performance claims, unverifiable superlatives, competitor brand names

If the user cannot supply a fact sheet, generate a draft from available information but clearly mark every unverified field with `[UNVERIFIED]`.

### Step 2 — Run the checklist

Load `references/checklist.md` and walk through sections 0–7 in order. For each item, mark pass or fail. Pay special attention to:

- Title: core information within the first 80 characters
- Bullets: exactly five, each opening with a 2–4 word capitalized benefit
- Main image: Amazon requires pure white background with no text; TikTok Shop allows scenario and social-proof elements
- Secondary images: prefer real product photos over AI-generated concept images; review each for text occlusion, incorrect expressions, and incomplete rendering
- Backend search terms: no repetition of title/bullets, no commas, under 250 bytes

Platform differences are summarized at the end of `references/checklist.md`.

### Step 3 — Rewrite copy

Use `references/before-after-example.md` as the style reference. The example uses bracketed placeholders (e.g. `Peak [X]W / RMS [Y]W`) — replace them with real values from the fact sheet.

Title structure: `Brand + core category keyword + key specs + scenario/benefit`
Bullet structure: `benefit (capitalized opener) → factual support → use scenario`

Replace vague claims with verifiable specifics: `sets up in 5 minutes` instead of `easy installation`.

### Step 4 — Pre-launch QA

Re-run section 7 of `references/checklist.md`. Verify that every number is consistent across title, bullets, images, and description. Check the mobile preview: title not truncated, bullet openers visible, image text readable. Confirm no competitor brand names, no unverifiable superlatives, and correct variant/price/stock linkage.

## Resources

- `references/checklist.md` — the complete 8-section QA checklist with pass/fail items, positive and negative examples, and a platform comparison table. Load during Step 2 and Step 4.
- `references/before-after-example.md` — a sanitized before/after rewrite with rationale for each change and an image review log. Load during Step 3 as the writing style reference.
- `assets/fact-sheet-template.md` — fillable fact sheet, one copy per SKU. Load during Step 1.
- `assets/title-workspace.md` — title rewrite worksheet with three candidate versions and a mobile preview field. Load during Step 3.

## Output Format

Deliver results in this order:

1. Fact sheet status (complete / fields still missing)
2. Checklist results table (section → pass/fail → issue)
3. Rewritten title (3 candidates) and five bullets
4. Image review notes
5. Pre-launch QA confirmation

Keep key e-commerce terms in English when the user communicates in Chinese.
