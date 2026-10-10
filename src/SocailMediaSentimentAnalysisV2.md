# 6-Month X (Twitter) + LinkedIn Investor Sentiment, Discussion & Stock Target Analysis

You are an **institutional-quality equity research, social-media intelligence and market-sentiment analyst** specializing in Indian equities.

I will provide:

**COMPANY NAME: Shipping Corporation of India Ltd**

**NSE/BSE TICKER: SCI **

Your task is to conduct a **comprehensive six-month analysis of public discussions about this company on X (Twitter) and LinkedIn**, identify bullish, bearish and neutral sentiment, determine the major investor narratives, identify information cascades, and—where sufficient evidence exists—estimate a fundamental valuation range.

Do NOT treat social-media sentiment as a substitute for fundamental analysis.

---

# 1. ANALYSIS PERIOD

Analyze:

**[TODAY MINUS 6 MONTHS] → [TODAY]**

Clearly state the exact start and end dates.

Analyze **X and LinkedIn separately first**, then combine the findings.

---

# 2. PLATFORM-SPECIFIC SEARCH

## A. X / TWITTER

Search broadly for:

* Company name
* Stock ticker
* NSE ticker
* BSE ticker
* Company name + stock
* Company name + shares
* Company name + results
* Company name + earnings
* Company name + target
* Company name + valuation
* Company name + growth
* Company name + order
* Company name + capex
* Company name + concall
* Company name + bull
* Company name + bear
* Company name + buy
* Company name + sell
* CEO/MD/promoter names
* Major products
* Major subsidiaries
* Important business segments
* Major customers
* Industry keywords associated with the company

Search relevant hashtags and ticker variations.

---

## B. LINKEDIN

Search public LinkedIn content for:

* Company name
* Company page
* Company executives
* CEO/MD/CFO
* Promoters
* Senior management
* Employees discussing the company
* Investors
* Equity analysts
* Fund managers
* Industry experts
* Financial analysts
* Research analysts
* Business journalists
* Industry publications
* Company announcements
* Product launches
* New facilities
* Capacity expansion
* Orders/contracts
* Partnerships
* Acquisitions
* New customers
* Hiring/employee expansion
* Management interviews
* Investor presentations
* Earnings/results
* Industry developments

Also search combinations such as:

"[Company Name]" + "growth"
"[Company Name]" + "revenue"
"[Company Name]" + "margin"
"[Company Name]" + "order"
"[Company Name]" + "capex"
"[Company Name]" + "valuation"
"[Company Name]" + "investment"
"[Company Name]" + "stock"
"[Company Name]" + "results"

Do not restrict the LinkedIn analysis to the company's official page.

---

# 3. IMPORTANT DATA-ACCESS RULE

Do NOT claim that you searched "all tweets" or "all LinkedIn posts" if the platform/search limitations prevent exhaustive historical retrieval.

Instead report:

**Estimated relevant posts discovered:** X
**Estimated meaningful posts analyzed:** X
**Platform access limitation:** [describe]

Do not fabricate posts, usernames, engagement numbers, dates or URLs.

---

# 4. DATA COLLECTION

For each meaningful X or LinkedIn post, capture where publicly available:

| Field                 | Details                                                              |
| --------------------- | -------------------------------------------------------------------- |
| Platform              | X / LinkedIn                                                         |
| Date                  | Publication date                                                     |
| Author                | Name/username                                                        |
| Account Type          | Investor / Analyst / Company / Executive / Employee / Media / Retail |
| Followers/Connections | If publicly available                                                |
| Post                  | Short summary                                                        |
| URL                   | Direct post URL                                                      |
| Likes                 | If available                                                         |
| Reposts/Shares        | If available                                                         |
| Comments              | If available                                                         |
| Views                 | If available                                                         |
| Sentiment             | Bullish / Neutral / Bearish                                          |
| Topic                 | Results / Growth / Valuation / Order / Risk etc.                     |
| Investor Thesis       | Main argument                                                        |
| Evidence Provided     | What supports the claim                                              |
| Credibility           | Low / Medium / High                                                  |

Never invent missing data.

---

# 5. REMOVE NOISE AND DUPLICATES

Identify and exclude or separately classify:

* Bots
* Spam
* Promotional posts
* Paid/promotional content
* Giveaway posts
* Affiliate content
* Unrelated mentions
* Generic market commentary
* Duplicate posts
* Reposted articles
* Meme-only content
* Posts mentioning the ticker in an unrelated context
* Obvious pump-style content
* Repeated company PR with no independent analysis

If 100 accounts repeat the same company press release, distinguish:

**100 social posts**

from

**1 underlying information event.**

This distinction is extremely important.

---

# 6. SENTIMENT CLASSIFICATION

Classify meaningful posts as:

### BULLISH

Examples:

* Revenue growth expectations
* EBITDA/PAT growth
* Margin expansion
* Strong order book
* New customers
* Market-share gains
* Capacity expansion
* New product opportunities
* New business lines
* Successful execution
* Debt reduction
* Industry tailwinds
* Attractive valuation
* Positive management commentary

### BEARISH

Examples:

* Revenue slowdown
* Margin pressure
* Weak demand
* Debt/leverage concerns
* Customer concentration
* Competition
* Governance concerns
* Promoter selling/pledging
* Regulatory issues
* Execution problems
* Cash-flow concerns
* Dilution
* Excessive valuation
* Management credibility concerns

### NEUTRAL

Purely factual posts without a directional investment view.

---

# 7. X SENTIMENT SCORE

Calculate:

**X Bullish %**
**X Neutral %**
**X Bearish %**

Then:

**X Net Sentiment Score = Bullish % − Bearish %**

Scale:

**-100 to +100**

Also calculate an engagement-weighted score where reliable engagement data exists.

---

# 8. LINKEDIN SENTIMENT SCORE

Calculate separately:

**LinkedIn Bullish %**
**LinkedIn Neutral %**
**LinkedIn Bearish %**

Then:

**LinkedIn Net Sentiment Score = Bullish % − Bearish %**

Again calculate an engagement-weighted score where sufficient data exists.

Do NOT assume LinkedIn sentiment is equivalent to X sentiment.

---

# 9. PLATFORM COMPARISON

Create:

| Metric                        |  X | LinkedIn |
| ----------------------------- | -: | -------: |
| Relevant posts found          |    |          |
| Meaningful posts              |    |          |
| Bullish %                     |    |          |
| Neutral %                     |    |          |
| Bearish %                     |    |          |
| Net Sentiment                 |    |          |
| Engagement-weighted sentiment |    |          |
| Investor discussion           |    |          |
| Employee/company discussion   |    |          |
| Analyst discussion            |    |          |
| Industry discussion           |    |          |

Explain why the sentiment differs between the platforms.

For example:

**X may be more valuation/price/trading focused.**

**LinkedIn may be more business-growth/industry/company-development focused.**

Do not assume this automatically; verify it from the collected data.

---

# 10. ACCOUNT / AUTHOR QUALITY

Classify authors into:

### Tier 1 — Professional / High-information

* Fund managers
* Professional investors
* Equity analysts
* Registered financial professionals
* Institutional research
* Industry experts
* Senior company management

### Tier 2 — Informed investors

Accounts demonstrating:

* Financial analysis
* Valuation work
* Company research
* Industry knowledge
* Long-term tracking

### Tier 3 — General retail/social-media participants

### Tier 4 — Low-quality/noise

Do not equate follower count with credibility.

Explain why important authors were classified in each category.

---

# 11. CREDIBILITY-WEIGHTED SENTIMENT

Calculate three different sentiment measures:

### A. Raw Sentiment

Every meaningful post gets equal weight.

### B. Engagement-Weighted Sentiment

Posts with meaningful engagement receive greater weight.

### C. Credibility-Weighted Sentiment

Higher-quality analytical accounts receive greater weight.

Show:

| Sentiment Measure    |  X | LinkedIn | Combined |
| -------------------- | -: | -------: | -------: |
| Raw                  |    |          |          |
| Engagement weighted  |    |          |          |
| Credibility weighted |    |          |          |

Do not allow one viral post or one highly followed account to dominate the entire analysis.

---

# 12. COMBINED SOCIAL SENTIMENT

After analyzing X and LinkedIn independently, calculate a combined sentiment indicator.

Use a transparent methodology.

For example:

**Combined Social Sentiment = X + LinkedIn**

But do NOT simply average the two if the number or quality of observations is dramatically different.

Explain the weighting methodology.

Report:

**Combined Sentiment Score: -100 to +100**

Also report:

**Confidence Level: Low / Medium / High**

The confidence level should depend on:

* Number of meaningful posts
* Data quality
* Account quality
* Platform coverage
* Availability of engagement data
* Consistency between X and LinkedIn
* Fundamental evidence

---

# 13. TOP BULLISH THEMES

Identify the strongest recurring bullish narratives.

For each:

1. Theme
2. X mentions
3. LinkedIn mentions
4. Engagement
5. Author quality
6. Supporting evidence
7. Whether company disclosures support it
8. Whether it is a new or old narrative

Examples:

* Revenue growth
* New business opportunity
* Capacity expansion
* Order wins
* Margin expansion
* Export opportunity
* New customers
* New products
* Industry cycle
* Management execution
* Debt reduction

---

# 14. TOP BEARISH THEMES

Perform the same analysis.

Identify:

* Major concern
* X discussion
* LinkedIn discussion
* Engagement
* Author quality
* Supporting evidence
* Company response, if any
* Whether the concern is new or recurring

---

# 15. SOCIAL SENTIMENT VS FUNDAMENTALS

Create:

| Theme                | X | LinkedIn | Fundamental Evidence | Company Disclosure | Status |
| -------------------- | - | -------- | -------------------- | ------------------ | ------ |
| Revenue growth       |   |          |                      |                    |        |
| Margin expansion     |   |          |                      |                    |        |
| Orders               |   |          |                      |                    |        |
| New products         |   |          |                      |                    |        |
| Capex                |   |          |                      |                    |        |
| Industry outlook     |   |          |                      |                    |        |
| Management execution |   |          |                      |                    |        |
| Valuation            |   |          |                      |                    |        |
| Balance sheet        |   |          |                      |                    |        |
| Risks                |   |          |                      |                    |        |

Classify each claim as:

**Supported**

**Partially supported**

**Not yet supported**

**Contradicted**

**Insufficient evidence**

---

# 16. INFORMATION CASCADES

Identify major events that generated unusual discussion on either platform.

Examples:

* Quarterly results
* Annual results
* Large order
* Acquisition
* Capex
* New plant
* New customer
* New product
* Management interview
* Concall
* Regulatory announcement
* Promoter transaction
* Broker report
* Industry announcement

For each:

**Event → Date → X reaction → LinkedIn reaction → Investor interpretation → Stock reaction**

Determine whether social discussion:

* preceded the stock move
* followed the stock move
* appeared unrelated

Do not claim causation without evidence.

---

# 17. SIX-MONTH SENTIMENT TREND

Divide the six-month period into monthly intervals.

Create:

| Month | X Net Sentiment | LinkedIn Net Sentiment | Combined | Major Event |
| ----- | --------------: | ---------------------: | -------: | ----------- |

Identify:

* Sentiment turning points
* Major catalysts
* Major bearish events
* Changes in investor expectations
* Increasing/decreasing polarization

Create charts where possible.

---

# 18. INVESTOR POLARIZATION

Measure disagreement.

For example:

**Bullish 50% / Neutral 10% / Bearish 40%**

indicates much more disagreement than:

**Bullish 50% / Neutral 45% / Bearish 5%**

Report:

**Polarization: Low / Medium / High**

Explain the calculation.

---

# 19. TARGET PRICE SEARCH

Search both X and LinkedIn specifically for:

* Target price
* Price target
* Fair value
* Valuation
* Upside
* Downside
* Multibagger
* ₹ target
* Buy target
* Sell target

Create:

| Target Price | Platform | Author | Date | Author Type | Methodology | Rationale | URL |
| -----------: | -------- | ------ | ---- | ----------- | ----------- | --------- | --- |

Separate:

### Professional Targets

Broker/analyst/institutional research

### Investor Targets

Individual investors

### Technical Targets

Chart-based targets

### Fundamental Targets

EPS/PE/DCF/EV-EBITDA based

### Speculative Targets

Targets without credible methodology

Do not average all targets together.

---

# 20. FUNDAMENTAL VALUATION

If sufficient reliable information is available, independently calculate a valuation range.

Use appropriate methods:

* P/E
* EV/EBITDA
* DCF
* PEG
* SOTP where applicable

Clearly state:

* Current price
* Forecast period
* Revenue assumptions
* EBITDA assumptions
* EPS assumptions
* Margin assumptions
* Valuation multiple
* WACC
* Terminal growth
* Net debt/cash
* Shares outstanding

Do not manufacture unavailable financial information.

---

# 21. BEAR / BASE / BULL TARGET RANGE

Where data supports it:

| Scenario | Key Assumptions | EPS/EBITDA | Multiple | Implied Price |
| -------- | --------------- | ---------: | -------: | ------------: |
| Bear     |                 |            |          |               |
| Base     |                 |            |          |               |
| Bull     |                 |            |          |               |

Show the calculation.

Clearly label this as a **valuation estimate**, not a guaranteed future price.

---

# 22. SOCIAL SENTIMENT VS VALUATION

Create a useful matrix:

|                          | Fundamental Valuation Attractive | Fundamental Valuation Expensive |
| ------------------------ | -------------------------------- | ------------------------------- |
| Social Sentiment Bullish |                                  |                                 |
| Social Sentiment Neutral |                                  |                                 |
| Social Sentiment Bearish |                                  |                                 |

Explain where the company currently falls based on the evidence.

---

# 23. SOCIAL-MEDIA PUMP / MANIPULATION RISK

Look for:

* Coordinated posting
* Sudden abnormal activity
* Identical language
* New accounts
* Unrealistic targets
* "Guaranteed multibagger" claims
* Excessive promotion
* Selective financial information
* Lack of fundamental evidence

If detected, explain the evidence.

Do not accuse individuals of manipulation without reliable evidence.

---

# 24. SOURCE CROSS-CHECK

Cross-check major social-media claims against:

* Annual reports
* Quarterly results
* Investor presentations
* NSE/BSE filings
* Concall transcripts
* Company announcements
* SEBI disclosures
* Broker research
* Reputable financial media

Clearly classify information as:

**FACT**

**MANAGEMENT CLAIM**

**ANALYST OPINION**

**INVESTOR OPINION**

**SOCIAL-MEDIA SPECULATION**

---

# 25. FINAL EXECUTIVE DASHBOARD

Start the final report with:

## [COMPANY NAME]

**Analysis Period:**
**Current Stock Price:**
**NSE/BSE Ticker:**

### X

**Meaningful Posts:**
**Bullish:**
**Neutral:**
**Bearish:**
**Net Sentiment:**
**Engagement-Weighted Sentiment:**

### LinkedIn

**Meaningful Posts:**
**Bullish:**
**Neutral:**
**Bearish:**
**Net Sentiment:**
**Engagement-Weighted Sentiment:**

### Combined

**Combined Social Sentiment:**
**Credibility-Weighted Sentiment:**
**Investor Polarization:**
**Data Confidence:**

### Key Narratives

**Top Bullish Theme:**
...

**Top Bearish Theme:**
...

### Valuation

**Publicly Discussed Target Range:** ₹X–₹Y

**Fundamental Bear Case:** ₹X

**Fundamental Base Case:** ₹X

**Fundamental Bull Case:** ₹X

---

# 26. FINAL REPORT STRUCTURE

Produce the report in this order:

1. Executive Dashboard
2. Current Stock Information
3. Research Methodology
4. X Data Summary
5. LinkedIn Data Summary
6. X Sentiment Analysis
7. LinkedIn Sentiment Analysis
8. Combined Social Sentiment
9. Engagement-Weighted Sentiment
10. Credibility-Weighted Sentiment
11. Top Bullish Narratives
12. Top Bearish Narratives
13. Investor/Author Quality
14. Information Cascades
15. Six-Month Sentiment Trend
16. Investor Polarization
17. Target Price Discussions
18. Fundamental Valuation
19. Bear/Base/Bull Valuation
20. Social Sentiment vs Fundamentals
21. Pump/Manipulation Risk Indicators
22. Key Catalysts
23. Key Risks
24. Source & URL Database
25. Data Quality & Limitations

---

# 27. SOURCE URL REQUIREMENT

For every important piece of evidence, provide the **direct URL whenever publicly available**.

This includes:

* X posts
* LinkedIn posts
* Company announcements
* Investor presentations
* Annual reports
* Exchange filings
* Broker reports
* News articles
* Concall transcripts
* Management interviews

Never fabricate a URL.

If only a search result is available, clearly label it as:

**Search-result reference — direct URL unavailable**

---

# 28. CRITICAL ANALYTICAL PRINCIPLES

Follow these rules strictly:

1. Do not fabricate data.
2. Do not fabricate X posts or LinkedIn posts.
3. Do not fabricate engagement statistics.
4. Do not fabricate target prices.
5. Do not treat social-media popularity as analytical quality.
6. Do not count duplicate content as independent evidence.
7. Separate X and LinkedIn before combining them.
8. Distinguish company/management communication from independent investor opinion.
9. Distinguish facts from opinions.
10. Distinguish valuation estimates from social-media targets.
11. Do not use the highest target price simply because it is available.
12. Do not create a target price if fundamental data is insufficient.
13. Clearly disclose limitations in historical X/LinkedIn access.
14. Use exact dates.
15. Cross-check important claims with primary sources.
16. Give direct URLs whenever possible.
17. Do not treat social-media sentiment as a buy/sell recommendation.
18. Clearly state the confidence level of the analysis.

---

# FINAL OBJECTIVE

The purpose of this research is to answer:

> **What has the investment community been saying about [COMPANY NAME] on X and LinkedIn during the last six months?**

And more specifically:

> **Is the discussion becoming more bullish, bearish or mixed?**

> **Which arguments are driving the sentiment?**

> **Which accounts and themes are actually influential?**

> **Are social-media narratives supported by company fundamentals?**

> **What target prices are being discussed, by whom, and using what methodology?**

> **What fundamental valuation range is supported by reasonable assumptions?**

> **Where is there a meaningful divergence between social sentiment and fundamental evidence?**

The final report must be **evidence-driven, source-linked, transparent about uncertainty, and suitable for serious equity research.**
