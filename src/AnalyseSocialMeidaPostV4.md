# NEW SECTION — SOCIAL MEDIA BULL–BEAR METER & SENTIMENT INTELLIGENCE

## OBJECTIVE

Create a dedicated **Social Media Bull–Bear Meter** using publicly discoverable and independently verifiable X and LinkedIn content.

The objective is NOT merely to count how many posts contain bullish or bearish words.

The objective is to determine:

> **What is the overall direction, intensity, quality and breadth of investor sentiment on X and LinkedIn, based on the actual substance of original posts and independent opinions?**

Calculate the Bull–Bear Meter separately for:

1. X
2. LinkedIn
3. Combined X + LinkedIn

The result must distinguish between:

**Sentiment Volume → Sentiment Strength → Engagement → Independent Voices → Information Quality → Final Bull/Bear Meter**

---

# 1. SENTIMENT CLASSIFICATION

Classify every sufficiently relevant original X post and LinkedIn post/comment into one of:

### STRONGLY BULLISH

Examples:

* Explicitly positive investment thesis
* Strong conviction that earnings/growth/valuation will improve
* Positive view supported by company-specific evidence
* Explicit buy/accumulation thesis
* Strongly positive interpretation of a catalyst

### BULLISH

Positive investment view with supporting reasoning but lower conviction.

### MILDLY BULLISH

Somewhat positive but with significant uncertainty.

### NEUTRAL / ANALYTICAL

Informational or balanced discussion without a clear directional investment view.

### MILDLY BEARISH

Somewhat negative but not strongly negative.

### BEARISH

Clearly negative investment thesis supported by reasoning.

### STRONGLY BEARISH

Strong negative thesis supported by company-specific evidence, valuation concerns, deteriorating fundamentals, governance concerns or other substantive evidence.

### NON-INVESTMENT / NOISE

Examples:

* Generic market commentary
* Memes
* Unrelated mentions
* Promotional content without substantive analysis
* Pure news sharing without an expressed view
* Irrelevant discussion

Do not include NOISE in the core sentiment calculation.

---

# 2. SENTIMENT SCORE FOR EACH POST

Assign a numerical sentiment score:

| Classification       |   Score |
| -------------------- | ------: |
| Strongly Bullish     |      +2 |
| Bullish              |      +1 |
| Mildly Bullish       |    +0.5 |
| Neutral / Analytical |       0 |
| Mildly Bearish       |    -0.5 |
| Bearish              |      -1 |
| Strongly Bearish     |      -2 |
| Noise / Irrelevant   | Exclude |

Do not classify a post as bullish merely because it contains words such as:

* Buy
* Target
* Multibagger
* Growth
* Order
* Defence
* Railway
* Breakout

Read the actual context.

Similarly, do not classify a post as bearish merely because it contains:

* Risk
* Debt
* Expensive
* Correction
* Sell
* Problem

Determine the actual investment view expressed in the post.

---

# 3. X SENTIMENT CALCULATION

For X, calculate:

### A. Sentiment Count

* Strongly Bullish
* Bullish
* Mildly Bullish
* Neutral
* Mildly Bearish
* Bearish
* Strongly Bearish
* Noise/Excluded

### B. Sentiment Percentage

Calculate:

**Bullish % = Bullish Posts / Total Sentiment-Classified Posts × 100**

where Bullish Posts include:

* Strongly Bullish
* Bullish
* Mildly Bullish

Calculate:

**Bearish % = Bearish Posts / Total Sentiment-Classified Posts × 100**

where Bearish Posts include:

* Strongly Bearish
* Bearish
* Mildly Bearish

Calculate:

**Neutral % = Neutral Posts / Total Sentiment-Classified Posts × 100**

The three percentages should approximately equal 100%.

---

# 4. X NET SENTIMENT SCORE

Calculate:

**Raw X Sentiment Score = Sum of individual sentiment scores / Number of sentiment-classified posts**

Normalize it to:

**X Sentiment Score = Raw Score × 50**

This produces a scale approximately from:

**-100 to +100**

Interpretation:

|       Score | Description                       |
| ----------: | --------------------------------- |
| +60 to +100 | Strongly Bullish Social Sentiment |
|  +25 to +59 | Bullish Social Sentiment          |
|  +10 to +24 | Mildly Bullish                    |
|    -9 to +9 | Neutral / Mixed                   |
|  -24 to -10 | Mildly Bearish                    |
|  -59 to -25 | Bearish                           |
| -100 to -60 | Strongly Bearish                  |

These are descriptive sentiment bands, NOT investment recommendations or price predictions.

---

# 5. LINKEDIN SENTIMENT CALCULATION

Perform exactly the same process for LinkedIn.

Calculate:

* Strongly Bullish %
* Bullish %
* Mildly Bullish %
* Neutral %
* Mildly Bearish %
* Bearish %
* Strongly Bearish %
* Noise %

Then calculate:

**LinkedIn Raw Sentiment Score**

and normalize it to:

**LinkedIn Sentiment Score: -100 to +100**

Use the same classification methodology as X.

---

# 6. BULL–BEAR METER

Create a visual/text-based meter for each platform.

Example:

**X BULL–BEAR METER**

`BEAR 0 ━━━━━━━━●━━━━━━━━ BULL 100`

Then show:

**Bullish: XX% | Neutral: XX% | Bearish: XX%**

**X Sentiment Score: +XX / -XX**

**Confidence: High / Medium / Low**

Repeat for LinkedIn.

Then create:

### COMBINED SOCIAL MEDIA BULL–BEAR METER

`BEAR 0 ━━━━━━━━━●━━━━━━━ BULL 100`

Show:

* X Bullish %
* X Bearish %
* LinkedIn Bullish %
* LinkedIn Bearish %
* Combined Bullish %
* Combined Bearish %
* Combined Neutral %
* Combined Social Sentiment Score
* Confidence

Do NOT simply average the raw number of posts if one platform has substantially better-quality evidence.

---

# 7. COMBINED SOCIAL SENTIMENT SCORE

Calculate the combined score using:

**X Social Sentiment Score = 60%**

**LinkedIn Social Sentiment Score = 40%**

unless the available sample size or quality makes this weighting inappropriate.

If the evidence quality differs substantially between platforms, adjust the weighting and explain why.

The final:

**Combined Social Sentiment Score = -100 to +100**

This score represents **social-media sentiment only**.

It must NOT be combined with fundamental or broker sentiment in this section.

---

# 8. ENGAGEMENT-WEIGHTED SENTIMENT

Do not assume every post has equal market influence.

Where engagement data is available, calculate a separate:

### Engagement-Weighted Sentiment

Consider:

* Likes
* Reposts/Retweets
* Replies
* Quote posts
* Views
* Comments
* Reactions
* Shares

Do NOT allow views to be treated as equivalent to likes or reposts.

Where sufficient data exists, calculate:

**Engagement-Weighted Sentiment = Σ(Post Sentiment × Engagement Weight) / Σ Engagement Weight**

Clearly explain the engagement weighting methodology used.

If engagement data is incomplete, state:

**Engagement-weighted sentiment could not be fully calculated.**

Do not estimate missing engagement.

---

# 9. INDEPENDENT-VOICE-ADJUSTED SENTIMENT

A major requirement:

> **100 bullish posts from 5 accounts should not be treated as equivalent to 100 bullish posts from 100 independent accounts.**

Calculate:

### Raw Sentiment

Based on sentiment-classified posts.

### Independent Sentiment

Deduplicate:

* Copy-paste posts
* Direct reposts
* Repeated broker reports
* Repeated news
* Identical narratives
* Coordinated promotional content

Then calculate sentiment using the remaining independent opinions.

Show:

| Metric                      |  X | LinkedIn |
| --------------------------- | -: | -------: |
| Raw Bullish %               |    |          |
| Raw Bearish %               |    |          |
| Independent Bullish %       |    |          |
| Independent Bearish %       |    |          |
| Neutral %                   |    |          |
| Sentiment Score             |    |          |
| Independent Sentiment Score |    |          |

---

# 10. INFORMATION-CASCADE-ADJUSTED SENTIMENT

Identify major sentiment narratives.

For each major narrative determine:

**Original Information → First Investor → Secondary Amplification → X → LinkedIn → Broader Narrative**

Example:

**Company Order Announcement → Analyst Interpretation → X Discussion → 25 Reposts → LinkedIn Discussion**

Treat this as one underlying information event rather than 25 independent bullish opinions.

Calculate:

### Raw Bullish Sentiment

before cascade adjustment.

### Cascade-Adjusted Bullish Sentiment

after removing duplicate/amplified opinions.

Do the same for bearish sentiment.

Show:

| Metric          | Raw | Cascade Adjusted |
| --------------- | --: | ---------------: |
| Bullish %       |     |                  |
| Bearish %       |     |                  |
| Neutral %       |     |                  |
| Sentiment Score |     |                  |

Explain major differences.

---

# 11. SENTIMENT QUALITY SCORE

Create a separate:

### Social Sentiment Quality Score: 0–100

Evaluate:

* Original research
* Company-specific evidence
* Financial analysis
* Professional contributors
* Independent voices
* Source transparency
* Evidence quality
* Historical reliability where verifiable
* Duplicate-content percentage
* Promotional-content percentage
* Information-cascade concentration

Do NOT interpret this as investment quality.

It measures the **quality of the social-media sentiment sample**.

---

# 12. BULL–BEAR SENTIMENT CONFIDENCE

Assign:

### HIGH CONFIDENCE

When:

* Large sample of independently verified posts
* Broad range of accounts
* Low duplication
* Strong original analysis
* Good engagement data
* Multiple independent narratives
* Consistent sentiment across different searches

### MEDIUM CONFIDENCE

When:

* Reasonable sample
* Some duplication
* Moderate professional participation
* Partial engagement information

### LOW CONFIDENCE

When:

* Small sample
* Highly concentrated accounts
* Significant reposting
* Heavy promotional content
* Poor discoverability
* Limited engagement information

Never provide a strong Bull–Bear Meter conclusion when confidence is LOW without explicitly highlighting the limitation.

---

# 13. SENTIMENT DIVERGENCE ANALYSIS

Compare:

### Raw Sentiment vs Independent Sentiment

### Post-Count Sentiment vs Engagement-Weighted Sentiment

### X Sentiment vs LinkedIn Sentiment

### Social Sentiment vs Fundamental Evidence

### Social Sentiment vs Broker Sentiment

Identify:

**Bullish Consensus**

**Bearish Consensus**

**Mixed Sentiment**

**Platform Divergence**

**Narrative Concentration**

**Contrarian Sentiment**

Example:

> X appears strongly bullish by post count, but after removing repeated content and weighting independent voices, sentiment is only mildly bullish.

Do not manufacture such a conclusion unless the data supports it.

---

# 14. SOCIAL MEDIA SENTIMENT TIME SERIES

Calculate the Bull–Bear Meter for:

### Last 30 Days

### Last 90 Days

### Last 6 Months

### Last 12 Months

Where sufficient data exists, show:

| Period    | Bullish % | Bearish % | Neutral % | Sentiment Score | Independent Score | Confidence |
| --------- | --------: | --------: | --------: | --------------: | ----------------: | ---------- |
| 30 Days   |           |           |           |                 |                   |            |
| 90 Days   |           |           |           |                 |                   |            |
| 6 Months  |           |           |           |                 |                   |            |
| 12 Months |           |           |           |                 |                   |            |

Identify:

* Sentiment improving
* Sentiment deteriorating
* Sentiment stable
* Bullish spike
* Bearish spike
* Sentiment reversal
* Sentiment divergence
* Sentiment becoming more concentrated

Identify the event responsible for significant changes wherever possible.

---

# 15. SENTIMENT × ENGAGEMENT MATRIX

Create:

| Platform | Bullish % | Bearish % | Neutral % | Avg Engagement | Bullish Engagement | Bearish Engagement | Sentiment Score |
| -------- | --------: | --------: | --------: | -------------: | -----------------: | -----------------: | --------------: |
| X        |           |           |           |                |                    |                    |                 |
| LinkedIn |           |           |           |                |                    |                    |                 |
| Combined |           |           |           |                |                    |                    |                 |

This must distinguish:

**How many people are saying it**

from:

**How much attention those opinions receive.**

---

# 16. SOCIAL MEDIA BULL–BEAR DASHBOARD

Create this mandatory dashboard:

| Metric                           |  X | LinkedIn | Combined |
| -------------------------------- | -: | -------: | -------: |
| Total Sentiment-Classified Posts |    |          |          |
| Strongly Bullish                 |    |          |          |
| Bullish                          |    |          |          |
| Mildly Bullish                   |    |          |          |
| Neutral                          |    |          |          |
| Mildly Bearish                   |    |          |          |
| Bearish                          |    |          |          |
| Strongly Bearish                 |    |          |          |
| Bullish %                        |    |          |          |
| Bearish %                        |    |          |          |
| Neutral %                        |    |          |          |
| Raw Sentiment Score              |    |          |          |
| Independent Sentiment Score      |    |          |          |
| Engagement-Weighted Score        |    |          |          |
| Cascade-Adjusted Score           |    |          |          |
| Sentiment Quality Score          |    |          |          |
| Confidence                       |    |          |          |

Then show:

### X BULL–BEAR METER

**Bear ←————————————→ Bull**

**Score: XX / 100**

### LINKEDIN BULL–BEAR METER

**Bear ←————————————→ Bull**

**Score: XX / 100**

### COMBINED SOCIAL BULL–BEAR METER

**Bear ←————————————→ Bull**

**Score: XX / 100**

---

# 17. BULLISH VS BEARISH NARRATIVE ANALYSIS

Identify the major narratives responsible for bullish and bearish sentiment.

### TOP BULLISH NARRATIVES

| Narrative | Number of Independent Voices | Engagement | Evidence | Cascade? | Confidence |
| --------- | ---------------------------: | ---------: | -------- | -------- | ---------- |

### TOP BEARISH NARRATIVES

| Narrative | Number of Independent Voices | Engagement | Evidence | Cascade? | Confidence |
| --------- | ---------------------------: | ---------: | -------- | -------- | ---------- |

For each major narrative identify:

* Original source
* Number of independent accounts
* Number of derivative posts
* Engagement
* Supporting evidence
* Contradicting evidence
* Whether it is fact, interpretation or speculation

---

# 18. SOCIAL SENTIMENT VS INFORMATION QUALITY

Create a final matrix:

| Signal                        | Finding |
| ----------------------------- | ------- |
| Raw Social Sentiment          |         |
| Independent Social Sentiment  |         |
| Engagement-Weighted Sentiment |         |
| Cascade-Adjusted Sentiment    |         |
| X Sentiment                   |         |
| LinkedIn Sentiment            |         |
| Professional Sentiment        |         |
| Retail Sentiment              |         |
| Bullish Narrative Strength    |         |
| Bearish Narrative Strength    |         |
| Sentiment Quality             |         |
| Sentiment Confidence          |         |

The purpose is to determine whether social sentiment is:

**Broad + Independent + Evidence-Based**

or

**Concentrated + Repetitive + Promotional/Speculative**

---

# 19. CRITICAL INTERPRETATION RULE

Never conclude:

> "The stock is bullish because social media is bullish."

Instead report:

> "Social-media sentiment is bullish/bearish/mixed based on the analysed sample, with X showing ___ sentiment and LinkedIn showing ___ sentiment. After adjusting for duplicate content, information cascades and engagement concentration, the sentiment changes to ___. The confidence level is ___. This is a social-media sentiment indicator and is not a price prediction."

---

# 20. SOCIAL MEDIA BULL–BEAR METER QUALITY CONTROL

Before finalizing the meter verify:

[ ] Every sentiment-classified post actually expresses an investment view

[ ] Sarcasm/context considered where reasonably detectable

[ ] News-only posts not automatically classified as bullish

[ ] Negative risk discussion not automatically classified as bearish

[ ] Bullish keywords not treated as bullish sentiment without context

[ ] Bearish keywords not treated as bearish sentiment without context

[ ] Reposts removed from independent sentiment

[ ] Copy-paste content removed

[ ] Information cascades identified

[ ] Duplicate narratives consolidated

[ ] Engagement separated from sentiment

[ ] Views not treated as equivalent to engagement

[ ] High-follower accounts not automatically given greater credibility

[ ] Professional identity verified where possible

[ ] Anonymous accounts not automatically discarded, but treated appropriately in credibility analysis

[ ] Raw sentiment calculated separately from adjusted sentiment

[ ] X and LinkedIn calculated separately

[ ] Combined sentiment methodology disclosed

[ ] Sentiment sample size disclosed

[ ] Confidence level disclosed

[ ] No missing data fabricated

[ ] No platform-wide sentiment claimed from an incomplete search

[ ] No sentiment score presented as a price prediction

---

# 21. FINAL SOCIAL MEDIA SENTIMENT STATEMENT

End the social-media section with exactly this structure:

### SOCIAL MEDIA BULL–BEAR METER

**X:** XX/100 — Bullish/Bearish/Neutral

**LinkedIn:** XX/100 — Bullish/Bearish/Neutral

**Combined:** XX/100 — Bullish/Bearish/Neutral

**Raw Bullish %:** XX%

**Raw Bearish %:** XX%

**Independent Bullish %:** XX%

**Independent Bearish %:** XX%

**Engagement-Weighted Sentiment:** XX

**Cascade-Adjusted Sentiment:** XX

**Sentiment Quality:** XX/100

**Confidence:** High/Medium/Low

### KEY OBSERVATION

Explain in 3–5 sentences:

1. What social media sentiment currently indicates
2. Whether X and LinkedIn agree
3. Whether sentiment survives duplicate/cascade adjustment
4. Which bullish and bearish narratives dominate
5. What evidence could cause the sentiment to change

Do NOT convert the Bull–Bear Meter into a buy/sell recommendation.
