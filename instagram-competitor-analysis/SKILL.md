---
name: instagram-competitor-analysis
description: Analyze public Instagram Reels from one or more competitor accounts and create an evidence-based Excel workbook with view tiers, content patterns, and recommendations. Use when the user requests competitor research or a reusable Instagram content-pattern library. Excludes private analytics, account management, carousels, Stories, and Lives.
---

# Instagram Competitor Analysis

Use this skill to analyze public Instagram **Reels only** and create a reusable Excel competitor-research workbook. Do not log in, request credentials, or use private analytics.

## Intake

Ask at the start of every run:

- Instagram profile URLs and/or usernames for each competitor.
- Niche or market being researched.
- Analysis objective: reach, engagement, authority, leads, or mixed.
- Number of recommendations wanted.
- Whether recommendations should use all competitors or selected tiers.

Use the last 90 days first. If fewer than 15 Reels are available, include older Reels until reaching 15. Use all available data if fewer than 15 exist. Exclude carousels, static posts, Stories, and Lives.

## Hard stop for missing views

Before analyzing an account, verify that public view/play counts are visible for the sampled Reels. If public views are unavailable for the page or Reel sample, **do not run analysis for that account**. Add a short limitation record: `Analysis not run: public view counts were unavailable.` Do not estimate views, assign Gold/Silver/Bronze tiers, or continue ranking that account.

## Ranking

Rank qualifying Reels by visible views/plays, descending. Use fixed thresholds:

- Gold: 100,000+ views
- Silver: 10,000-99,999 views
- Bronze: under 10,000 views

Do not force five rows into a tier. A tier can contain fewer rows or be empty. Preserve the sample size. If a Reel has no public views, it cannot be ranked; record the limitation and exclude it from the ranked set.

## Workbook deliverable

Create an `.xlsx` workbook with sortable/filterable tables and separate tabs:

- `Read Me` - scope, date, methodology, thresholds, and exclusions.
- `Intake` - run-specific inputs.
- One tab per competitor - ranked Reel table followed by key findings.
- `Combined Pattern Library` - consolidated patterns with competitor-specific variations.
- `Strategic Takeaways` - cross-competitor themes and evidence limits.
- `Recommendations` - the requested number of evidence-linked recommendations.
- `Evidence Limitations` - accounts/posts excluded or not run.

Use the detailed schema in [references/workbook-schema.md](references/workbook-schema.md). Keep row text concise: observations under 20 words and likely-performance explanations under 35 words. Do not repeat competitor names in every explanation when the tab name already identifies them.

## Required Reel columns

Every competitor tab must include:

`Tier, Rank, Reel URL, Posted date, Views/plays, Likes, Comments, Shares, Duration, Format, Topic, Audience, CTA, Sentiment, Hook type, Visual hook, Verbal hook, Written hook, Hook keywords, Topic keywords, Audience keywords, CTA keywords, Direct observation, Why it likely performed, Evidence status, Pattern ID.`

Use controlled values where possible. Default vocabularies are documented in the schema reference. Keep four keyword fields separate. Put concise, evidence-based interpretation in the observation fields.

## Key findings below each competitor table

Include exactly these fields:

- What consistently works
- What underperforms
- Pattern to adapt
- Do not copy
- Evidence limitation

Use `Not enough in-period evidence` when appropriate. Do not invent performance conclusions.

## Pattern library and recommendations

When the same pattern appears across competitors, create one consolidated Pattern ID and preserve competitor-specific variations and all source Reel URLs beneath it. Each recommendation must include the source competitor(s), source Reel URL(s), tier, observed pattern, recommended adaptation, and any `Do not copy` constraint.

Keep client relevance out of this standalone competitor-analysis skill. Recommendations should be based on observed competitor patterns and the run's stated niche/market and objective, without pretending to know a client's audience or offer.

## Spreadsheet design

Use formulas for tier assignment, table filters, and conditional formatting. Gold should use Burgundy, Silver Blush, and Bronze a neutral/mint treatment. Do not add charts by default. Use an `Evidence status` field with `Visible` or `Unavailable`; never fabricate hidden metrics.

Before delivering, verify that every competitor tab has the requested sample, visible view evidence, correct thresholds, links, key findings, and limitations. Save the workbook with a descriptive filename and report any account that triggered the hard stop.
