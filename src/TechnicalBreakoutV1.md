# GEMINI PRO — NSE MULTI-BREAKOUT STOCK SCANNER

## USER INPUT — PASTE YOUR STOCK LIST BELOW

Replace the example stocks below with your own list.

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

* The stocks between START STOCK LIST and END STOCK LIST are the ONLY stocks to analyse.
* Analyse EVERY stock provided.
* Do not add stocks that are not present in the input list.
* Do not remove stocks from the input list unless the stock is delisted or the ticker cannot be reliably identified.
* If only company names are provided, identify the correct NSE ticker.
* If both company name and ticker are provided, verify that they match.
* If the ticker is incorrect, report the corrected ticker instead of silently changing it.

---

# YOUR ROLE

Act as a quantitative technical analyst specialising in Indian equities and the NSE market.

Your task is to scan the stocks provided in the USER INPUT section and identify which stocks are currently showing **at least one technical breakout** using the seven breakout strategies defined below.

The objective is:

> Identify stocks from MY PROVIDED LIST that are currently showing one or more technically valid breakouts.

Do not analyse the entire NSE universe.

Analyse ONLY the stocks supplied between START STOCK LIST and END STOCK LIST.

---

# ANALYSIS DATE

First determine the latest available NSE trading date.

Clearly state:

* Analysis date
* Last available trading session
* Data timestamp, if available

Use the same analysis date for all stocks.

Do not mix current data with data from different dates.

---

# STEP 1 — VERIFY INPUT STOCKS

Create an initial verification table:

| Input Company | Input Ticker | Verified Company | Verified NSE Ticker | Status                             |
| ------------- | ------------ | ---------------- | ------------------- | ---------------------------------- |
| ...           | ...          | ...              | ...                 | Verified / Corrected / Unavailable |

If a ticker is corrected, clearly explain why.

If a stock cannot be reliably identified, mark:

DATA UNAVAILABLE

Do not guess.

---

# STEP 2 — MARKET REGIME

Before analysing individual stocks, analyse:

* NIFTY 50
* NIFTY 500

Check:

* Current price vs 50 DMA
* Current price vs 200 DMA
* 50 DMA vs 200 DMA
* Recent momentum
* Recent volatility

Classify the current market environment as:

* Trending Up
* Range Bound
* Trending Down
* High Volatility
* Unclear

This is contextual information only.

Do not use it to remove stocks from the scan.

---

# STEP 3 — ANALYSE EVERY STOCK

For EACH stock in the input list, test ALL seven breakout strategies.

---

# BREAKOUT STRATEGY 1 — 52-WEEK HIGH

Check:

Current closing price > previous 52-week high

Confirm:

* Previous 52-week high
* Current price
* Breakout date
* Volume ratio
* Percentage above previous 52-week high

Prefer volume:

Breakout volume ≥ 1.5 × 20-day average volume

Classify:

* Confirmed
* Developing
* Failed/Invalid
* No Breakout

---

# BREAKOUT STRATEGY 2 — CONSOLIDATION / RANGE BREAKOUT

Look for a clearly identifiable 4–12 week consolidation.

Identify:

* Range high
* Range low
* Approximate consolidation duration
* Resistance level
* Number of resistance tests
* Breakout price
* Breakout date
* Current price
* Breakout volume

Prefer:

Breakout volume ≥ 1.5 × 20-day average volume

Do not classify an ordinary price rise as a consolidation breakout.

---

# BREAKOUT STRATEGY 3 — DARVAS BOX

Identify whether the stock has formed a recognizable Darvas-style price box.

Check:

* Box high
* Box low
* Multiple reactions near upper boundary
* Price remaining within the box
* Breakout above box high
* Volume confirmation

Report:

* Box high
* Box low
* Breakout price
* Breakout date
* Current price
* Volume ratio

---

# BREAKOUT STRATEGY 4 — DONCHIAN

Test BOTH:

### 20-Day Donchian

Current close > previous 20-day high

### 55-Day Donchian

Current close > previous 55-day high

Report separately:

* Donchian 20: Confirmed / No
* Donchian 55: Confirmed / No

If both are triggered, explicitly highlight this.

---

# BREAKOUT STRATEGY 5 — EMA + PRICE BREAKOUT

Check:

* Price > 20 EMA
* Price > 50 EMA
* 20 EMA > 50 EMA
* 50 EMA > 200 EMA

IMPORTANT:

Being above moving averages alone is NOT sufficient.

There must also be a recent breakout above meaningful resistance or a major swing high.

Report:

* Current price
* 20 EMA
* 50 EMA
* 200 EMA
* Resistance
* Breakout date
* Distance from 50 EMA
* Distance from 200 EMA

---

# BREAKOUT STRATEGY 6 — BOLLINGER SQUEEZE

Use:

* 20-period Bollinger Bands
* 2 standard deviations

Look for:

1. Volatility contraction
2. Narrow Bollinger Band width
3. Subsequent volatility expansion
4. Price breaking above upper Bollinger Band
5. Preferably increased volume

Report:

* Upper Bollinger Band
* Bollinger Band width
* Previous compression period
* Current price
* Volume ratio
* Breakout date

---

# BREAKOUT STRATEGY 7 — SUPPORT / RESISTANCE BREAKOUT

Identify significant horizontal resistance.

Look for:

* Multiple previous tests
* Clear resistance
* Closing price above resistance
* Volume confirmation

Report:

* Resistance
* Number of previous tests
* Breakout price
* Current price
* Breakout date
* Volume ratio

---

# STEP 4 — BREAKOUT CONFIRMATION

For each breakout check:

## PRICE

* Close above resistance
* Breakout above recent swing high
* Breakout above 20-day high
* Breakout above 55-day high
* Breakout above 52-week high

## VOLUME

Calculate:

Breakout Volume ÷ 20-Day Average Volume

Classify:

* <1.0 = Weak
* 1.0–1.5 = Moderate
* ≥1.5 = Strong
* ≥2.0 = Very Strong

If the stock is illiquid, explain the limitation.

## TREND

Check:

* Price > 20 EMA
* Price > 50 EMA
* 20 EMA > 50 EMA
* 50 EMA > 200 EMA

## MOMENTUM

Calculate:

* RSI(14)
* 1-month return
* 3-month return
* 6-month return

Do not automatically reject an otherwise valid breakout because RSI is above 70.

---

# STEP 5 — RELATIVE STRENGTH

Compare each stock with NIFTY 500.

Calculate:

* 1-month performance
* 3-month performance
* 6-month performance

Classify:

* Outperforming NIFTY 500
* In line
* Underperforming NIFTY 500

Highlight:

BREAKOUT + NIFTY 500 OUTPERFORMANCE

---

# STEP 6 — BREAKOUT COUNT

For every stock calculate:

Breakout Count = Number of the seven strategies currently confirming a breakout.

Possible:

0 to 7

Use:

✓ = Confirmed

~ = Developing/Potential

✗ = No Breakout

IMPORTANT:

Any stock with:

Breakout Count ≥ 1

must be included in the final breakout results.

---

# STEP 7 — MULTI-BREAKOUT CONFLUENCE

Identify stocks where multiple strategies confirm the same move.

Examples:

* 52-week high + 55-day Donchian
* Consolidation + volume breakout
* Darvas + 52-week high
* Bollinger squeeze + resistance breakout
* Donchian + EMA trend

Explain the actual evidence.

Do not falsely describe correlated signals as completely independent confirmations.

---

# STEP 8 — FALSE BREAKOUT ANALYSIS

For every breakout check:

* Close back below resistance
* Weak volume
* Large upper wick
* Immediate reversal
* Poor follow-through
* Previous failed breakout
* Excessive extension

Flag:

Potential False Breakout

where appropriate.

---

# STEP 9 — OVEREXTENSION

Calculate:

* Distance from 20 EMA
* Distance from 50 EMA
* Distance from 200 EMA

Classify:

* Not Extended
* Moderately Extended
* Highly Extended

This is only a risk/context flag.

Do not reject a valid breakout solely because the stock is extended.

---

# STEP 10 — BREAKOUT FRESHNESS

Classify every confirmed breakout as:

* Latest trading session
* Within last 3 trading sessions
* Within last 5 trading sessions
* More than 5 sessions ago

Provide the exact breakout date whenever possible.

---

# OUTPUT 1 — STOCK VERIFICATION

First show:

| Input Stock | Input Ticker | Verified NSE Stock | Verified Ticker | Status |
| ----------- | ------------ | ------------------ | --------------- | ------ |

This proves that every input stock was processed.

---

# OUTPUT 2 — MASTER BREAKOUT TABLE

Show EVERY stock having at least one confirmed or developing breakout.

| Stock | NSE | Price | Breakout Count | 52W | Range | Darvas | D20 | D55 | EMA | BB Squeeze | S/R | Volume Ratio | RSI | Relative Strength | Breakout Date | Status |
| ----- | --- | ----: | -------------: | --- | ----- | ------ | --- | --- | --- | ---------- | --- | -----------: | --: | ----------------- | ------------- | ------ |

Use:

✓ = Confirmed

~ = Developing

✗ = No

Sort by:

1. Breakout Count
2. Volume confirmation
3. Relative strength
4. Breakout freshness

This is an analytical ordering, NOT an investment ranking.

---

# OUTPUT 3 — STOCKS WITH 2 OR MORE BREAKOUTS

Create:

| Stock | NSE | Breakout Count | Confirmed Strategies | Breakout Date | Volume Ratio | RSI | Trend | Relative Strength | Extension | Risk Flags |
| ----- | --- | -------------: | -------------------- | ------------- | -----------: | --: | ----- | ----------------- | --------- | ---------- |

For each stock give a short explanation of the technical confluence.

---

# OUTPUT 4 — STOCKS WITH EXACTLY 1 BREAKOUT

Create:

| Stock | NSE | Breakout Type | Breakout Price | Current Price | Date | Volume Ratio | RSI | Relative Strength | Risk Flags |
| ----- | --- | ------------- | -------------: | ------------: | ---- | -----------: | --: | ----------------- | ---------- |

Do not exclude these stocks.

---

# OUTPUT 5 — FRESH BREAKOUTS

Show stocks whose breakout occurred during the last five trading sessions.

| Stock | Breakout Type | Date | Breakout Price | Current Price | Volume Ratio | RSI | Relative Strength |
| ----- | ------------- | ---- | -------------: | ------------: | -----------: | --: | ----------------- |

---

# OUTPUT 6 — NEAR-BREAKOUT WATCHLIST

From the ORIGINAL INPUT LIST, identify stocks that have NOT broken out but are close to significant resistance.

Use approximately:

Current price within 5% of important resistance.

Show:

| Stock | Current Price | Resistance | Distance % | Volume Trend | RSI | 20 EMA | 50 EMA | Relative Strength |
| ----- | ------------: | ---------: | ---------: | ------------ | --: | -----: | -----: | ----------------- |

Clearly label:

NOT YET A BREAKOUT

---

# OUTPUT 7 — RISK FLAGS

List relevant technical concerns:

* Weak volume
* Excessive extension
* Previous failed breakout
* Weak relative strength
* Immediate resistance
* High volatility
* Poor market regime
* Low liquidity

---

# OUTPUT 8 — DATA QUALITY

For every stock:

High / Medium / Low

Explain any data limitations.

Never invent missing data.

Use:

Data Unavailable

where reliable information cannot be obtained.

---

# SOURCES

Search the web for current and historical market information.

Prioritise:

1. NSE
2. BSE
3. Company filings
4. Reliable market-data providers
5. Established financial websites

Provide source citations and clickable URLs for important data.

Do not rely only on search-result snippets.

If sources disagree, explain the discrepancy.

---

# FINAL SUMMARY

End with:

## MARKET REGIME

NIFTY 50:
NIFTY 500:

Market environment:

---

## SCAN SUMMARY

Analysis date:

Total stocks supplied:

Total stocks successfully analysed:

Data unavailable:

Stocks with ≥1 breakout:

Stocks with ≥2 breakouts:

Fresh breakouts:

Potential false breakouts:

Near-breakout stocks:

---

## MULTI-BREAKOUT STOCKS

List the stocks with ≥2 confirmed breakout strategies and briefly describe the technical evidence.

---

## FRESH BREAKOUTS

List the stocks that broke out within the last five trading sessions.

---

## IMPORTANT TECHNICAL RISK FLAGS

List stocks where breakout confirmation has meaningful technical concerns.

---

# VERY IMPORTANT FINAL RULES

* Analyse ONLY the stocks between START STOCK LIST and END STOCK LIST.
* Analyse EVERY stock in that section.
* Never silently omit a stock.
* Never invent technical data.
* Never predict future prices.
* Never provide buy/sell recommendations.
* Never assign investment scores or ratings.
* Do not call a price increase a breakout without technical evidence.
* Clearly distinguish confirmed, developing and failed breakouts.
* Show the evidence supporting every breakout.
* Use the latest available trading data.
* Use the same analysis date for all stocks.
* Cite important data sources.
* If data is unavailable, explicitly say so.
* Remember that multiple indicators may be measuring the same underlying price movement.

The final objective is simply:

**FROM MY PROVIDED STOCK LIST, IDENTIFY WHICH STOCKS CURRENTLY SHOW AT LEAST ONE OF THE 7 DEFINED BREAKOUT PATTERNS, AND SHOW THE TECHNICAL EVIDENCE FOR EACH.**
