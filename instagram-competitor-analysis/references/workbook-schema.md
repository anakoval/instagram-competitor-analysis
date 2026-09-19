# Workbook schema

Use this reference when building the Excel workbook.

## Competitor tab columns

| Column | Entry rule |
|---|---|
| Tier | Formula from visible views: Gold 100,000+; Silver 10,000-99,999; Bronze under 10,000. |
| Rank | Descending visible views within the analyzed sample. |
| Reel URL | Direct public Reel URL. |
| Posted date | Public posting date; preserve the displayed date if exact date is unavailable. |
| Views/plays | Publicly visible count only. No estimates. |
| Likes / Comments / Shares | Visible counts; use `Unavailable` when not public. |
| Duration | Publicly visible duration where available. |
| Format | `Talking head`, `Interview`, `Podcast clip`, `Property tour`, `Listing walkthrough`, `Testimonial`, `Screen recording`, `Text-led`, `B-roll`, `Slideshow`, `Live clip`, `Reaction`, or `Tutorial`. |
| Topic | Concise subject label. |
| Audience | Best-supported audience label. |
| CTA | `DM`, `Comment`, `Save`, `Share`, `Follow`, `Click link`, `Book call`, `Download guide`, or `None`. |
| Sentiment | `Aspirational`, `Educational`, `Urgent`, `Emotional`, `Humorous`, `Controversial`, `Reassuring`, `Authoritative`, or `Practical`. |
| Hook type | `Question`, `Bold claim`, `Warning`, `Curiosity gap`, `Statistic`, `Story`, `Mistake`, `Comparison`, `Prediction`, or `Challenge`. |
| Visual hook | Short visible description. |
| Verbal hook | Opening spoken hook, paraphrased. |
| Written hook | Opening on-screen/caption hook, paraphrased. |
| Hook keywords | Four to eight concise terms. |
| Topic keywords | Four to eight concise terms. |
| Audience keywords | Four to eight concise terms. |
| CTA keywords | Exact CTA terms or paraphrases. |
| Direct observation | Under 20 words; only what is visible. |
| Why it likely performed | Under 35 words; clearly framed as an inference. |
| Evidence status | `Visible` or `Unavailable`. |
| Pattern ID | Stable ID such as `P-01`, reused for recurring patterns. |

## Summary fields

Below each competitor table, add exactly:

- What consistently works
- What underperforms
- Pattern to adapt
- Do not copy
- Evidence limitation

Use concise prose and cite Reel URLs in the evidence or source columns. If evidence is thin, say `Not enough in-period evidence` rather than generalizing.

## Pattern library columns

`Pattern ID, Pattern name, Shared pattern, Competitors observed, Source Reel URLs, Tier evidence, Competitor-specific variations, Recommended adaptation, Do not copy, Evidence limitation.`

## Recommendations columns

`Recommendation ID, Recommendation, Objective, Pattern ID, Source competitor(s), Source Reel URL(s), Tier, Format, Hook type, Topic, Audience, CTA, Why this is recommended, Do not copy, Evidence status.`

## Workbook rules

- Keep one row per Reel.
- Rank Reels together by visible views; do not include carousels.
- Do not force a fixed number of rows into tiers.
- Use Excel tables with filters and freeze the header row.
- Use formulas for tier assignment and conditional formatting for tier colors.
- Do not add charts unless the user asks for them.
- Keep observations compact to reduce repeated text and preserve workbook usability.
