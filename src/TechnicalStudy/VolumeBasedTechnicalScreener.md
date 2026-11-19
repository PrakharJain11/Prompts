# GEMINI PRO — NSE VOLUME, PRICE & BUYER ACCUMULATION SCANNER

## USER INPUT — STOCK LIST

Paste my stocks between the following markers.

### START STOCK LIST

```text
Tega Industries | TEGA
Bharat Heavy Electricals Ltd. | BHEL
BEML Ltd. | BEML
Viyash Scientific Ltd. | VIYASH
Motilal Oswal Financial Services Ltd. | MOTILALOFS
Pricol Ltd | PRICOL
Skipper Ltd | SKIPPER
Jana Small Finance Bank Ltd. | JANASFB
RBL Bank Ltd.| RBLBANK
Aarti Pharmalabs Ltd. | AARTIPHARM
Eureka Forbes Ltd. | EUREKAFORB
V.S.T. Tillers Tractors Ltd. | VSTTILLERS
Sandur Manganese & Iron Ores Ltd. | SANDUMA
Fedbank Financial Services Ltd | FEDFINA
Northern ARC Capital Ltd. | NORTHERNARC
Happy Forgings Ltd. | HAPPYFORGE
Xpro India Ltd. | XPROINDIA
Sansera Engineering Ltd. | SANSERA
Gokaldas Exports Ltd. | GOKEX
IIFL Finance Ltd. | IIFL
Borosil Renewables Ltd. | BORORENEW
Wockhardt Ltd. | WOCKPHARMA
```

### END STOCK LIST

IMPORTANT:

* Analyse ONLY the stocks between START STOCK LIST and END STOCK LIST.
* Analyse EVERY stock provided.
* Do not add stocks that are not in my list.
* Do not silently omit any stock.
* If only company names are provided, identify the correct NSE ticker.
* If both company name and ticker are provided, verify that they match.
* If a stock cannot be reliably identified, mark it as DATA UNAVAILABLE.

---

# ROLE

Act as a **quantitative Indian equity analyst specialising in volume-price analysis, accumulation/distribution, market microstructure, FII/DII activity and investor behaviour**.

My objective is to identify stocks from my provided list where there is evidence of:

1. Increasing trading volume
2. Increasing price
3. Increasing delivery/holding conviction
4. Buyers becoming stronger than sellers
5. Possible accumulation by institutions, large investors or other informed participants
6. Ideally, decreasing retail participation while institutional/large-investor participation is increasing

Do NOT simply look for stocks whose prices increased.

I want to identify **stocks where price + volume + participation are moving together in a potentially bullish manner.**

---

# ANALYSIS PERIOD

Use:

### Primary period

The latest completed 5 trading sessions / approximately 1 trading week.

Compare this with:

### Comparison period

The previous 5 trading sessions.

Also examine:

* 20-day average
* 50-day average, where useful

Clearly state the:

* Analysis date
* Last trading date
* Primary 1-week period
* Previous 1-week comparison period

Do not compare incomplete trading sessions.

---

# STEP 1 — PRICE ANALYSIS

For every stock calculate:

### 1-week:

* Opening price
* Closing price
* Highest price
* Lowest price
* 1-week return %

Compare with:

* Previous week's closing price
* Previous 5-day return
* 20-day performance
* NIFTY 500 performance over the same period

Calculate:

### Price Change %

```text
(Current 5-day close - Previous 5-day close)
÷ Previous 5-day close × 100
```

Classify:

* Strongly Increasing
* Increasing
* Flat
* Decreasing

---

# STEP 2 — VOLUME ANALYSIS

For every stock calculate:

### Current week average daily volume

versus:

### Previous week average daily volume

Also compare current volume with:

* 20-day average volume
* 50-day average volume, where available

Calculate:

### Volume Change %

```text
(Current 5-day average volume
-
Previous 5-day average volume)
÷ Previous 5-day average volume × 100
```

Also calculate:

### Volume Ratio

```text
Current 5-day average volume
÷
20-day average daily volume
```

Classify volume:

* Strong Increase
* Moderate Increase
* Normal
* Decrease

Pay particular attention to:

> Price ↑ + Volume ↑

This is more important than price increase alone.

---

# STEP 3 — DAILY VOLUME-PRICE RELATIONSHIP

Do not analyse only weekly averages.

For each of the latest five sessions examine:

| Date | Close Change % | Volume | Volume vs 20DMA | Delivery % | Delivery Volume | Interpretation |
| ---- | -------------: | -----: | --------------: | ---------: | --------------: | -------------- |

Look for patterns such as:

### Bullish accumulation pattern

Price ↑
Volume ↑
Delivery ↑

### Possible distribution

Price ↓
Volume ↑
Delivery ↑

### Weak rally

Price ↑
Volume ↓

### Possible short-term trading activity

Price ↑
Volume ↑
Delivery ↓

Explain which pattern is present.

---

# STEP 4 — DELIVERY DATA

For NSE stocks, analyse delivery information wherever reliable data is available.

Look at:

* Delivery quantity
* Delivery percentage
* Delivery volume
* Delivery trend
* Delivery vs 20-day average

Calculate:

### Delivery Volume Change

Current week's average delivery quantity vs previous week's average delivery quantity.

### Delivery Percentage Change

Current average delivery % vs previous average delivery %.

Pay particular attention to:

> Price ↑ + Volume ↑ + Delivery ↑

This combination should receive stronger accumulation attention.

However:

IMPORTANT:

Delivery data does NOT directly prove that institutions are buying.

Treat it as evidence of increased positional participation, not proof of institutional accumulation.

---

# STEP 5 — BUYER VS SELLER STRENGTH

Determine whether there is evidence that buying pressure is stronger than selling pressure.

Use ALL reliable information available, including:

* Price action
* Volume
* Delivery
* Intraday price structure
* Closing position within daily range
* Bid/ask information if available
* Market depth if available
* Trade data if available
* Block deals
* Bulk deals
* Institutional disclosures

For each stock determine:

### Buyer/Seller Pressure

Classify as:

* Strong Buyer Dominance
* Moderate Buyer Dominance
* Balanced
* Moderate Seller Dominance
* Strong Seller Dominance
* Insufficient Data

---

# IMPORTANT BUYER/SELLER RULE

Do NOT claim:

"Buyers are greater than sellers"

merely because the price increased.

Price increase alone does NOT prove that the number of buyers exceeded sellers.

Instead, look for multiple pieces of evidence.

For example:

Price ↑
Volume ↑
Delivery ↑
Positive closing near day's high
Strong relative performance
Positive block/bulk activity

would provide stronger evidence of buying pressure.

---

# STEP 6 — INTRADAY BUYER STRENGTH

Where reliable intraday data is available, examine:

* Opening price
* High
* Low
* Close
* VWAP
* Volume
* Closing location within day's range

Look for:

### Strong accumulation characteristics

* Price holding above VWAP
* Repeated buying near VWAP/support
* Close near day's high
* High volume on upward candles
* Lower volume on pullbacks

### Distribution characteristics

* High volume on down days
* Repeated rejection from higher prices
* Close near day's low
* High-volume selling
* Price below VWAP

Do not fabricate order-book data if it is unavailable.

---

# STEP 7 — RETAIL VS INSTITUTIONAL PARTICIPATION

This is a VERY IMPORTANT part of the analysis.

Determine whether there is evidence that:

### Retail participation is decreasing

AND/OR

### Institutional / large-investor participation is increasing.

Use the following evidence sources.

---

## A. SHAREHOLDING PATTERN

Check the latest available quarterly shareholding pattern.

Compare at least:

* Latest quarter
* Previous quarter
* Preferably previous 2–4 quarters

Look at:

### Promoters

* Holding %
* Change

### FII/FPI

* Holding %
* Change

### DII

* Holding %
* Change

### Mutual Funds

* Holding %
* Change

### Insurance companies

* Holding %
* Change

### Banks / financial institutions

* Holding %
* Change

### Public / retail shareholders

* Holding %
* Change

### Number of shareholders

If available, examine the change in number of shareholders.

---

# STEP 8 — RETAIL INVESTOR ANALYSIS

Do NOT automatically assume:

Public shareholders = retail investors.

Instead, clearly distinguish between:

* Retail investors, if specifically disclosed
* Public shareholders
* Non-institutional public
* Other shareholders

Look for:

### Potential retail reduction

* Declining retail/public ownership %
* Declining number of small shareholders
* Increasing average holding size, if calculable
* Institutional ownership increasing simultaneously

If reliable retail-specific data is unavailable, state:

"Retail participation cannot be directly established from available public data."

Do NOT guess.

---

# STEP 9 — INSTITUTIONAL ACCUMULATION

Analyse:

### FII/FPI

* Current holding
* Previous holding
* Change
* Recent buying/selling if available

### DII

* Current holding
* Previous holding
* Change

### Mutual Funds

* Holding change
* Number of schemes holding the stock, if available

### Insurance / Banks / Institutions

* Holding change

Also search for:

* Institutional buying
* Block deals
* Bulk deals
* Mutual fund transactions
* FII/DII activity
* Major institutional investors entering/exiting

---

# STEP 10 — BLOCK & BULK DEAL ANALYSIS

Search for recent:

* Bulk deals
* Block deals

Look at the latest 1–3 months.

For each relevant deal report:

* Date
* Buyer
* Seller
* Quantity
* Price
* Approximate transaction value
* Whether buyer is institutional
* Whether seller is institutional

Pay particular attention to:

### Institutional Buyer + Rising Price + Rising Volume

This can be stronger evidence of accumulation.

However, do NOT automatically interpret every block/bulk deal as bullish.

Explain the context.

---

# STEP 11 — INSTITUTIONAL OWNERSHIP TREND

Create a simple trend:

| Quarter | FII % | DII % | MF % | Public/Retail % | Promoter % |
| ------- | ----: | ----: | ---: | --------------: | ---------: |

Then identify:

### Institutional Accumulation

if institutional ownership is increasing.

### Institutional Distribution

if institutional ownership is decreasing.

### Stable

if changes are insignificant.

---

# STEP 12 — PRICE + VOLUME + PARTICIPATION CONFLUENCE

Identify stocks satisfying combinations such as:

### Strong Accumulation

Price ↑
Volume ↑
Delivery ↑
Institutional holding ↑

### Possible Accumulation

Price ↑
Volume ↑
Delivery ↑

but institutional data is not yet available.

### Possible Distribution

Price ↓
Volume ↑
Delivery ↑
Institutional holding ↓

### Weak Price Rise

Price ↑
Volume ↓
Delivery ↓

---

# STEP 13 — RELATIVE STRENGTH

Compare every stock against:

* NIFTY 50
* NIFTY 500
* Relevant sector index where available

Calculate:

* 1-week relative performance
* 1-month relative performance
* 3-month relative performance

Identify:

### Strong

Stock outperforming NIFTY 500 while volume is increasing.

---

# STEP 14 — TECHNICAL TREND CONFIRMATION

Check:

* Price > 20 EMA
* Price > 50 EMA
* Price > 200 EMA
* 20 EMA > 50 EMA
* 50 EMA > 200 EMA
* RSI(14)
* MACD trend, where useful

The purpose is to determine whether increasing volume is occurring:

### Inside an established uptrend

or

### During a potential trend reversal

or

### During a temporary spike.

---

# STEP 15 — VOLUME SPIKE DETECTION

Identify stocks where:

Current volume is significantly above normal.

Calculate:

### Volume Spike Ratio

```text
Latest 5-day average volume
÷
20-day average volume
```

Also identify individual sessions where:

Daily volume ≥ 2 × 20-day average volume

Report:

* Date
* Volume
* Volume ratio
* Price change
* Delivery %
* Closing position

---

# STEP 16 — ACCUMULATION VS DISTRIBUTION

For every stock classify:

### Strong Accumulation

or

### Moderate Accumulation

or

### Neutral

or

### Moderate Distribution

or

### Strong Distribution

or

### Insufficient Data

Explain the evidence.

Do not make this classification based on one indicator.

Use multiple data points.

---

# STEP 17 — MAIN OUTPUT TABLE

Create the following table for ALL stocks showing meaningful improvement in price and/or volume:

| Stock | NSE | 1W Price % | Volume Change % | Volume Ratio | Delivery Change | RSI | Relative Strength | Buyer/Seller Pressure | Institutional Trend | Retail Trend | Accumulation/Distribution |
| ----- | --- | ---------: | --------------: | -----------: | --------------: | --: | ----------------- | --------------------- | ------------------- | ------------ | ------------------------- |

---

# STEP 18 — TOP ACCUMULATION CANDIDATES

Create a separate section containing stocks where the strongest combination of evidence exists.

Prioritise:

1. Price increasing
2. Volume increasing
3. Delivery increasing
4. Relative strength positive
5. Institutional ownership increasing
6. FII/DII/MF accumulation
7. Positive bulk/block deals
8. Buyer pressure stronger than seller pressure
9. Retail participation potentially declining

Do NOT create an arbitrary numerical score.

Instead, explain the evidence for each stock.

Example format:

### STOCK NAME — NSE:TICKER

**Price:** +X% in 1 week
**Volume:** +X%
**Volume vs 20DMA:** X×
**Delivery:** +X%
**Relative strength:** Outperforming NIFTY 500

**Institutional evidence:**

* FII: ↑
* DII: ↑
* Mutual Funds: ↑

**Retail evidence:**

* Public/retail holding: ↓ / ↑ / Unclear

**Buyer/Seller evidence:**
Strong / Moderate / Balanced / Weak

**Conclusion:**
Strong evidence of accumulation / Moderate evidence / Insufficient evidence

---

# STEP 19 — RETAIL EXIT + INSTITUTIONAL ENTRY

Create a SPECIAL WATCHLIST containing stocks where there is evidence of:

### Retail participation decreasing

AND

### Institutional / large investor participation increasing

AND preferably:

### Price increasing

AND

### Volume increasing

Use the latest available quarterly ownership data.

For every stock clearly state:

* What evidence suggests retail participation is decreasing?
* What evidence suggests institutions are increasing?
* How recent is the evidence?
* Is the evidence direct or indirect?

IMPORTANT:

If the data does not actually support the conclusion, say:

"NOT CONFIRMED"

rather than forcing a conclusion.

---

# STEP 20 — SMART MONEY EVIDENCE

Create another section showing stocks with evidence of possible large-investor accumulation.

Consider:

* FII buying
* DII buying
* Mutual fund buying
* Insurance company buying
* Large institutional shareholders increasing
* Block deals
* Bulk deals
* Prominent investors increasing holdings
* Large shareholder additions

Clearly distinguish:

### Confirmed institutional activity

from

### Possible accumulation inferred from price/volume data.

---

# STEP 21 — WARNING / FALSE SIGNALS

Identify stocks where:

* Price increased but volume decreased
* Volume increased but price decreased
* Volume spike appears speculative
* Delivery decreased
* Institutional ownership decreased
* Large shareholder exited
* Stock is highly volatile
* Price is already excessively extended
* Increase appears to be caused by a single news event
* Liquidity is poor

These should NOT be classified as strong accumulation.

---

# STEP 22 — DATA QUALITY

For every stock classify:

### Data Quality

High / Medium / Low

Also specify if:

* Delivery data unavailable
* Institutional data outdated
* Retail data unavailable
* Bulk/block deal data unavailable
* Intraday order-book data unavailable

Never estimate missing data.

---

# SOURCE HIERARCHY

Prefer these sources:

### Highest priority

1. NSE
2. BSE
3. Company investor presentations
4. Company annual reports
5. Company quarterly filings
6. SEBI disclosures
7. Exchange bulk/block deal disclosures

### Secondary

8. Moneycontrol
9. Screener
10. Trendlyne
11. Tijori Finance
12. Economic Times
13. Business Standard
14. Financial Express
15. Other established financial-data providers

Use the most recent available data.

Provide citations/links for important claims.

---

# IMPORTANT DATA INTERPRETATION RULES

## DO NOT SAY:

"Buyers are more than sellers because price increased."

Price is determined by executed trades and does not directly provide the number of buyers versus sellers.

Instead say:

"Price, volume, delivery and market-depth/trade data indicate stronger buying pressure."

only when the evidence supports it.

---

## DO NOT SAY:

"Retail investors are selling."

unless reliable shareholder-level evidence supports it.

Instead say:

"Public/retail ownership declined according to the latest shareholding disclosure."

---

## DO NOT SAY:

"Institutions are accumulating."

unless institutional ownership, transactions, bulk/block deals or other reliable evidence supports it.

If only price/volume data suggests accumulation, say:

"Possible accumulation based on price-volume-delivery behaviour; institutional participation is not confirmed."

---

# FINAL SUMMARY

End the report with:

## 1. STRONG ACCUMULATION

Stocks showing the strongest combination of:

Price ↑ + Volume ↑ + Delivery ↑ + Relative Strength ↑

and preferably institutional accumulation.

---

## 2. POSSIBLE INSTITUTIONAL ACCUMULATION

Stocks where there is evidence of FII/DII/MF/institutional buying or large-investor activity.

---

## 3. RETAIL ↓ + INSTITUTIONAL ↑

Stocks where available ownership/shareholder data indicates:

Retail/Public participation ↓

AND

Institutional participation ↑

Clearly identify whether this is:

Confirmed

or

Potential / Indirect Evidence.

---

## 4. PRICE + VOLUME BREAKOUT

Stocks where:

Price ↑

AND

Volume ↑ significantly

but institutional participation is not confirmed.

---

## 5. POSSIBLE DISTRIBUTION

Stocks where:

Volume ↑

but price action and participation data indicate selling/distribution.

---

## 6. NO CLEAR SIGNAL

Stocks where the available data does not provide meaningful evidence of accumulation or distribution.

---

# FINAL DASHBOARD

Provide this summary:

| Metric                                 | Result |
| -------------------------------------- | -----: |
| Total stocks provided                  |        |
| Successfully analysed                  |        |
| Data unavailable                       |        |
| Price increasing                       |        |
| Volume increasing                      |        |
| Price + Volume increasing              |        |
| Price + Volume + Delivery increasing   |        |
| Strong accumulation                    |        |
| Possible accumulation                  |        |
| Institutional accumulation confirmed   |        |
| Retail/Public participation decreasing |        |
| Retail ↓ + Institutional ↑             |        |
| Possible distribution                  |        |

---

# FINAL OBJECTIVE

The ultimate objective is NOT simply to find stocks whose prices increased.

Find stocks where the following sequence is visible:

**Price ↑

* Volume ↑
* Delivery ↑
* Relative Strength ↑
* Buying pressure ↑
* Institutional participation ↑
* Retail participation ↓ (where reliably measurable)**

The more independent evidence supporting the accumulation thesis, the stronger the finding.

However, never manufacture evidence.

If retail vs institutional participation cannot be reliably determined from available data, explicitly say:

**"Not determinable from available public data."**

This is a market-research and screening exercise, not investment advice.
