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

---

# IMPORTANT — STOCK UNIVERSE RESTRICTION

The stocks between START STOCK LIST and END STOCK LIST are the **ONLY stocks to analyse**.

* Analyse EVERY stock provided.
* Do not add stocks that are not in the input list.
* Do not remove stocks unless delisted or the ticker cannot be reliably identified.
* If only company names are provided, identify the correct NSE ticker.
* If both company name and ticker are provided, verify that they match.
* If the ticker is incorrect, report the corrected ticker.
* Never silently replace an input stock.

---

# YOUR ROLE

Act as a **quantitative technical analyst specialising in Indian equities and NSE markets**.

Your objective is to identify which stocks from MY PROVIDED LIST are currently showing one or more technically valid breakout setups.

You must analyse **ONLY the supplied stocks**.

---

# CRITICAL TIMEFRAME RULE

## USE ONLY DAILY AND WEEKLY CHARTS

For ALL breakout strategies:

### Allowed timeframes:

* **Daily (1D)**
* **Weekly (1W)**

### STRICTLY PROHIBITED:

* Monthly chart
* Monthly breakout
* Monthly resistance
* Monthly confirmation
* Monthly trend signal

**DO NOT USE MONTHLY CHART DATA FOR ANY PART OF THE BREAKOUT SCAN.**

If a monthly chart happens to be available from a data source, completely ignore it.

For every breakout, explicitly state:

**Timeframe: Daily / Weekly**

When both Daily and Weekly confirm the same breakout, mark:

**Daily + Weekly Confirmed**

---

# ANALYSIS DATE

First determine the latest available NSE trading date.

Clearly state:

* Analysis date
* Last available trading session
* Data timestamp, if available

Use the **same analysis date** for all stocks.

Do not mix data from different trading dates.

For weekly calculations, use the latest **completed weekly candle** where appropriate.

For daily calculations, use the latest completed trading session.

---

# STEP 1 — VERIFY INPUT STOCKS

Create:

| Input Company | Input Ticker | Verified Company | Verified NSE Ticker | Status                             |
| ------------- | ------------ | ---------------- | ------------------- | ---------------------------------- |
| ...           | ...          | ...              | ...                 | Verified / Corrected / Unavailable |

If a ticker is corrected, explain why.

If a stock cannot be reliably identified:

**DATA UNAVAILABLE**

Do not guess.

---

# STEP 2 — MARKET REGIME

Analyse:

* NIFTY 50
* NIFTY 500

Use ONLY:

* Daily chart
* Weekly chart

Check:

* Current price vs 50 DMA
* Current price vs 200 DMA
* 50 DMA vs 200 DMA
* Recent momentum
* Recent volatility
* Weekly trend

Classify:

* Trending Up
* Range Bound
* Trending Down
* High Volatility
* Unclear

This is contextual information only.

Do NOT use market regime to remove stocks from the scan.

---

# STEP 3 — ANALYSE EVERY STOCK

For EACH stock:

Test ALL **8 breakout strategies**.

Each strategy must be independently evaluated.

The eight strategies are:

1. 52-Week High
2. Consolidation / Range Breakout
3. Darvas Box
4. Donchian
5. EMA + Price Breakout
6. Bollinger Squeeze
7. Support / Resistance Breakout
8. **Prakhar’s Algorithm**

---

# BREAKOUT STRATEGY 1 — 52-WEEK HIGH

Use Daily and Weekly data.

Check:

**Current closing price > previous 52-week high**

Confirm:

* Previous 52-week high
* Current price
* Breakout date
* Timeframe
* Breakout volume
* 20-day average volume
* Volume ratio
* Percentage above previous 52-week high

Preferred confirmation:

**Breakout volume ≥ 1.5 × 20-day average volume**

Classify:

* Confirmed
* Developing
* Failed / Invalid
* No Breakout

---

# BREAKOUT STRATEGY 2 — CONSOLIDATION / RANGE BREAKOUT

Identify a clearly defined **4–12 week consolidation** using Daily/Weekly price action.

Identify:

* Range high
* Range low
* Consolidation duration
* Resistance
* Number of resistance tests
* Breakout price
* Breakout date
* Current price
* Breakout volume
* Timeframe

Preferred:

**Breakout volume ≥ 1.5 × 20-day average volume**

Do NOT classify an ordinary price rise as a consolidation breakout.

---

# BREAKOUT STRATEGY 3 — DARVAS BOX

Identify recognizable Darvas-style price action.

Check:

* Box high
* Box low
* Multiple reactions near upper boundary
* Price remaining inside box
* Breakout above box high
* Volume confirmation
* Timeframe

Report:

* Box high
* Box low
* Breakout price
* Breakout date
* Current price
* Volume ratio
* Daily/Weekly confirmation

---

# BREAKOUT STRATEGY 4 — DONCHIAN

Test both:

## 20-DAY DONCHIAN

Current close > previous 20-day high

## 55-DAY DONCHIAN

Current close > previous 55-day high

Report separately:

* D20: Confirmed / Developing / No
* D55: Confirmed / Developing / No

If both trigger:

**20D + 55D DONCHIAN CONFIRMED**

Also identify whether the signal is supported by the Weekly chart.

---

# BREAKOUT STRATEGY 5 — EMA + PRICE BREAKOUT

Check:

* Price > 20 EMA
* Price > 50 EMA
* 20 EMA > 50 EMA
* 50 EMA > 200 EMA

IMPORTANT:

Being above moving averages alone is NOT a breakout.

There must also be a recent breakout above meaningful resistance or a major swing high.

Report:

* Current price
* 20 EMA
* 50 EMA
* 200 EMA
* Resistance
* Breakout date
* Timeframe
* Distance from 50 EMA
* Distance from 200 EMA

---

# BREAKOUT STRATEGY 6 — BOLLINGER SQUEEZE

Use:

* 20-period Bollinger Bands
* 2 standard deviations

Use Daily and Weekly charts.

Look for:

1. Volatility contraction
2. Narrow Bollinger Band width
3. Subsequent volatility expansion
4. Price breaking above upper Bollinger Band
5. Preferably increased volume

Report:

* Upper Bollinger Band
* Bollinger Band width
* Compression period
* Current price
* Volume ratio
* Breakout date
* Timeframe

---

# BREAKOUT STRATEGY 7 — SUPPORT / RESISTANCE BREAKOUT

Identify significant horizontal resistance using Daily/Weekly price action.

Look for:

* Multiple previous tests
* Clear resistance
* Closing price above resistance
* Volume confirmation
* Follow-through

Report:

* Resistance
* Number of previous tests
* Breakout price
* Current price
* Breakout date
* Volume ratio
* Timeframe

---

# BREAKOUT STRATEGY 8 — PRAKHAR'S ALGORITHM

## PURPOSE

This is a dedicated momentum + volume breakout strategy.

The strategy consists of **FOUR CONDITIONS**.

A stock is considered to have a:

### PRAKHAR ALGORITHM CONFIRMED BREAKOUT

ONLY when **ALL FOUR conditions are satisfied on the same timeframe and within a reasonably close signal window.**

Test this strategy separately on:

* **Daily chart**
* **Weekly chart**

DO NOT use the Monthly chart.

---

## PRAKHAR CONDITION 1 — SUPERTREND TURNS GREEN

Use a standard Supertrend indicator.

Check whether:

**Supertrend has changed from RED → GREEN**

The important signal is the **transition**, not simply that Supertrend is already green.

Report:

* Previous Supertrend state
* Current Supertrend state
* Date of RED → GREEN transition
* Current price
* Daily / Weekly timeframe

Classify:

* Fresh Turn Green
* Already Green
* No Signal

A stock that has been green for a long time should NOT receive a fresh Supertrend breakout signal merely because the current Supertrend remains green.

---

## PRAKHAR CONDITION 2 — 8-PERIOD EMA OF ON-BALANCE VOLUME

Use:

**Indicator: On-Balance Volume (OBV)**

Apply:

**Moving Average**

Parameters:

* Period = **8**
* Source / Field = **OBV**
* Type = **Exponential (EMA)**
* Offset = **8**, if supported by the charting platform

The primary purpose is to identify strengthening OBV momentum.

Report:

* Current OBV
* 8-period EMA of OBV
* OBV vs 8 EMA
* Direction of OBV EMA
* Daily / Weekly timeframe

---

## PRAKHAR CONDITION 3 — OBV CROSSOVER

Check for:

**OBV crossing ABOVE its 8-period EMA**

This should be treated as a momentum confirmation.

Report:

* Previous OBV relationship to EMA
* Current OBV relationship to EMA
* Crossover date
* Crossover direction
* Timeframe

Classify:

* Fresh Bullish Crossover
* Bullish but not fresh
* No Crossover
* Bearish

### IMPORTANT

Do NOT consider:

**OBV > EMA**

alone to be a fresh crossover.

The strategy specifically requires:

**OBV crossing from BELOW → ABOVE its 8 EMA.**

---

# PRAKHAR CONDITION 4 — RSI CROSSES 66

Use:

**RSI period = 14**

Check for:

**RSI crossing ABOVE 66**

The important signal is:

Previous RSI ≤ 66

AND

Current RSI > 66

Report:

* Previous RSI
* Current RSI
* RSI crossover date
* Daily / Weekly timeframe

Classify:

* Fresh Cross Above 66
* Already Above 66
* Below 66
* Failed Cross

### IMPORTANT

Do NOT classify a stock as having a fresh RSI signal merely because:

**RSI > 66**

The RSI must actually cross **above 66**.

---

# PRAKHAR'S ALGORITHM — FINAL LOGIC

For each timeframe separately:

### DAILY PRAKHAR SIGNAL

A Daily Prakhar Breakout is confirmed when:

**Supertrend RED → GREEN**

AND

**OBV crosses ABOVE its 8-period EMA**

AND

**RSI(14) crosses ABOVE 66**

AND

**Price action supports an upward breakout / momentum move**

within a reasonably close signal window.

---

### WEEKLY PRAKHAR SIGNAL

A Weekly Prakhar Breakout is confirmed when:

**Weekly Supertrend RED → GREEN**

AND

**Weekly OBV crosses ABOVE its 8-period EMA**

AND

**Weekly RSI(14) crosses ABOVE 66**

AND

**Price action supports an upward breakout / momentum move**

within a reasonably close signal window.

---

# PRAKHAR SIGNAL WINDOW

Because different indicators may trigger on slightly different candles, allow a maximum signal window of:

### 3 trading sessions on Daily

or

### 2 completed weekly candles on Weekly

However:

The closer the signals occur, the stronger the setup.

Report:

* Days/candles between Supertrend signal
* OBV crossover
* RSI 66 crossover

Classify:

### Strong Prakhar Signal

All conditions trigger very close together and price confirms breakout.

### Confirmed Prakhar Signal

All four conditions are satisfied within the permitted signal window.

### Developing Prakhar Signal

2–3 conditions are satisfied and the remaining condition is close.

### Invalid Prakhar Signal

Conditions occurred too far apart or momentum subsequently failed.

---

# PRAKHAR ALGORITHM — IMPORTANT INTERPRETATION

Do NOT artificially manufacture a signal.

For example:

If:

* Supertrend is already green
* OBV is already above EMA
* RSI is already above 66

but none of these recently crossed,

DO NOT call it a fresh Prakhar breakout.

Instead report:

**Prakhar conditions currently positive, but no fresh Prakhar crossover signal.**

This distinction is extremely important.

---

# PRAKHAR ALGORITHM — STRENGTH LEVEL

Assign a signal strength based on the evidence.

### VERY STRONG

* All 4 conditions confirmed
* Fresh signals
* Strong price breakout
* Strong volume
* Daily + Weekly confirmation

### STRONG

* All 4 conditions confirmed
* Fresh signals
* Price breakout confirmed
* Good volume

### MODERATE

* All 4 conditions confirmed
* But weak volume or extended price

### DEVELOPING

* 2–3 conditions confirmed
* Remaining condition close to triggering

### NOT CONFIRMED

* Conditions do not align

Do NOT treat these as investment ratings.

They are only technical signal-strength classifications.

---

# PRAKHAR ALGORITHM — REQUIRED OUTPUT

For every stock where Prakhar's Algorithm is Confirmed or Developing, show:

| Stock | Timeframe | Supertrend | OBV | OBV 8 EMA | OBV Cross | RSI | RSI >66 Cross | Price Breakout | Signal Window | Prakhar Status |
| ----- | --------- | ---------- | --: | --------: | --------- | --: | ------------- | -------------- | ------------- | -------------- |

Use:

✓ = Confirmed

~ = Developing

✗ = Not confirmed

---

# STEP 4 — BREAKOUT CONFIRMATION

For every breakout check:

## PRICE

* Close above resistance
* Breakout above recent swing high
* Breakout above 20-day high
* Breakout above 55-day high
* Breakout above 52-week high

## VOLUME

Calculate:

**Breakout Volume ÷ 20-Day Average Volume**

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

Compare every stock against NIFTY 500.

Calculate:

* 1-month performance
* 3-month performance
* 6-month performance

Classify:

* Outperforming NIFTY 500
* In line
* Underperforming NIFTY 500

Highlight:

**BREAKOUT + NIFTY 500 OUTPERFORMANCE**

---

# STEP 6 — BREAKOUT COUNT

For every stock calculate:

**Breakout Count = Number of the 8 strategies currently confirming a breakout**

Possible:

**0 to 8**

Use:

✓ = Confirmed

~ = Developing

✗ = No Breakout

IMPORTANT:

Any stock with:

**Breakout Count ≥ 1**

must be included in the final breakout results.

---

# IMPORTANT — PRAKHAR ALGORITHM COUNTING

If Prakhar's Algorithm is confirmed, count it as:

**ONE breakout strategy**

Do NOT count each of its four conditions as separate breakout strategies.

For example:

Supertrend ✓
OBV crossover ✓
RSI >66 ✓

These together produce:

**Prakhar Algorithm = 1 confirmed strategy**

not 3.

---

# STEP 7 — MULTI-BREAKOUT CONFLUENCE

Identify stocks where multiple strategies confirm the same move.

Examples:

* 52-week High + 55-day Donchian
* Consolidation + Volume Breakout
* Darvas + 52-week High
* Bollinger Squeeze + Resistance Breakout
* Donchian + EMA Trend
* **Prakhar Algorithm + 52-week High**
* **Prakhar Algorithm + Donchian**
* **Prakhar Algorithm + Consolidation Breakout**
* **Prakhar Algorithm + Support/Resistance Breakout**

Explain the actual evidence.

Do not falsely describe correlated indicators as completely independent confirmations.

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

**Potential False Breakout**

where appropriate.

For Prakhar Algorithm also check whether:

* Supertrend turned green but quickly reversed
* OBV crossover failed
* RSI crossed 66 but fell back below
* Price failed to follow through

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

Do not reject a valid breakout solely because the stock is extended.

---

# STEP 10 — BREAKOUT FRESHNESS

Classify every confirmed breakout:

* Latest trading session
* Within last 3 trading sessions
* Within last 5 trading sessions
* More than 5 sessions ago

Provide exact breakout date whenever possible.

For Prakhar Algorithm additionally report:

* Supertrend signal date
* OBV crossover date
* RSI 66 crossover date
* Price breakout date

---

# OUTPUT 1 — STOCK VERIFICATION

| Input Stock | Input Ticker | Verified NSE Stock | Verified Ticker | Status |
| ----------- | ------------ | ------------------ | --------------- | ------ |

This proves every input stock was processed.

---

# OUTPUT 2 — MASTER BREAKOUT TABLE

Show EVERY stock having at least one confirmed or developing breakout.

| Stock | NSE | Price | Breakout Count | 52W | Range | Darvas | D20 | D55 | EMA | BB Squeeze | S/R | Prakhar | Volume Ratio | RSI | Relative Strength | Breakout Date | Timeframe | Status |
| ----- | --- | ----: | -------------: | --- | ----- | ------ | --- | --- | --- | ---------- | --- | ------- | -----------: | --: | ----------------- | ------------- | --------- | ------ |

Use:

✓ = Confirmed

~ = Developing

✗ = No

Sort by:

1. Breakout Count
2. Prakhar Algorithm confirmation
3. Volume confirmation
4. Relative strength
5. Breakout freshness

This is an analytical ordering, NOT an investment ranking.

---

# OUTPUT 3 — STOCKS WITH 2 OR MORE BREAKOUTS

| Stock | NSE | Breakout Count | Confirmed Strategies | Prakhar | Breakout Date | Volume Ratio | RSI | Trend | Relative Strength | Extension | Risk Flags |
| ----- | --- | -------------: | -------------------- | ------- | ------------- | -----------: | --: | ----- | ----------------- | --------- | ---------- |

For each stock provide a short explanation of the technical confluence.

---

# OUTPUT 4 — PRAKHAR ALGORITHM RESULTS

This section is mandatory.

Show:

### CONFIRMED PRAKHAR SIGNALS

| Stock | Timeframe | Supertrend Turn | OBV Cross | RSI Cross 66 | Price Breakout | Volume | Signal Window | Strength |
| ----- | --------- | --------------- | --------- | ------------ | -------------- | ------ | ------------- | -------- |

Then:

### DEVELOPING PRAKHAR SIGNALS

| Stock | Timeframe | Conditions Met | Missing Condition | Current RSI | OBV vs EMA | Supertrend | Price Status |
| ----- | --------- | -------------: | ----------------- | ----------: | ---------- | ---------- | ------------ |

Then:

### PRAKHAR SIGNALS THAT FAILED

Show recently triggered signals that subsequently failed.

---

# OUTPUT 5 — STOCKS WITH EXACTLY 1 BREAKOUT

| Stock | NSE | Breakout Type | Breakout Price | Current Price | Date | Timeframe | Volume Ratio | RSI | Relative Strength | Risk Flags |
| ----- | --- | ------------- | -------------: | ------------: | ---- | --------- | -----------: | --: | ----------------- | ---------- |

Do not exclude these stocks.

---

# OUTPUT 6 — FRESH BREAKOUTS

Show stocks whose breakout occurred during the last five trading sessions.

| Stock | Breakout Type | Date | Breakout Price | Current Price | Timeframe | Volume Ratio | RSI | Relative Strength |
| ----- | ------------- | ---- | -------------: | ------------: | --------- | -----------: | --: | ----------------- |

---

# OUTPUT 7 — NEAR-BREAKOUT WATCHLIST

From the ORIGINAL INPUT LIST, identify stocks that have NOT broken out but are close to significant resistance.

Use approximately:

**Current price within 5% of important resistance.**

Show:

| Stock | Current Price | Resistance | Distance % | Volume Trend | RSI | 20 EMA | 50 EMA | Relative Strength |
| ----- | ------------: | ---------: | ---------: | ------------ | --: | -----: | -----: | ----------------- |

Clearly label:

**NOT YET A BREAKOUT**

Also identify whether Prakhar's Algorithm is:

* 0/4 conditions
* 1/4
* 2/4
* 3/4
* 4/4 but breakout not yet confirmed

---

# OUTPUT 8 — RISK FLAGS

List relevant technical concerns:

* Weak volume
* Excessive extension
* Previous failed breakout
* Weak relative strength
* Immediate resistance
* High volatility
* Poor market regime
* Low liquidity
* Prakhar signal failure
* RSI failed above 66
* OBV crossover failed
* Supertrend reversal

---

# OUTPUT 9 — DATA QUALITY

For every stock:

**High / Medium / Low**

Explain data limitations.

Never invent missing data.

Use:

**Data Unavailable**

where reliable information cannot be obtained.

---

# OUTPUT 10 — DAILY VS WEEKLY BREAKOUT ALIGNMENT

This is important.

Identify stocks where the breakout is confirmed on:

### Daily only

### Weekly only

### Daily + Weekly

Create:

| Stock | Strategy | Daily | Weekly | Alignment | Strength |
| ----- | -------- | ----- | ------ | --------- | -------- |

Give special attention to:

**Daily + Weekly confirmation**

because this represents stronger multi-timeframe technical alignment.

Do NOT use Monthly charts.

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

# DATA VALIDATION RULE

Technical indicators must be calculated from reliable historical OHLCV data whenever possible.

Do NOT simply copy a website's "Buy/Sell" signal.

Where possible, independently calculate:

* EMA
* RSI
* OBV
* OBV EMA
* Supertrend
* Bollinger Bands
* Donchian levels
* Volume ratios

If an indicator cannot be independently calculated, clearly state:

**Indicator data unavailable / externally sourced**

Do not fabricate the value.

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

Prakhar Algorithm confirmed:

Prakhar Algorithm developing:

Daily + Weekly confirmed:

Potential false breakouts:

Near-breakout stocks:

---

# MULTI-BREAKOUT STOCKS

List stocks with ≥2 confirmed breakout strategies.

Briefly describe the technical evidence.

---

# PRAKHAR ALGORITHM — TOP SIGNALS

List stocks where the four Prakhar conditions have aligned.

For each:

* Stock
* Timeframe
* Supertrend RED → GREEN date
* OBV crossover date
* RSI >66 crossover date
* Price breakout
* Volume
* Signal window
* Whether Daily + Weekly agree

---

# FRESH BREAKOUTS

List stocks that broke out within the last five trading sessions.

---

# DAILY + WEEKLY CONFIRMATION

List stocks where Daily and Weekly charts independently support the breakout.

---

# IMPORTANT TECHNICAL RISK FLAGS

List stocks where breakout confirmation has meaningful technical concerns.

---

# VERY IMPORTANT FINAL RULES

* Analyse ONLY stocks between START STOCK LIST and END STOCK LIST.
* Analyse EVERY stock.
* Never silently omit a stock.
* Never invent technical data.
* Never predict future prices.
* Never provide buy/sell recommendations.
* Never assign investment scores or ratings.
* Do not call a price increase a breakout without technical evidence.
* Clearly distinguish Confirmed, Developing and Failed breakouts.
* Show evidence supporting every breakout.
* Use latest available trading data.
* Use the same analysis date for all stocks.
* Cite important data sources.
* If data is unavailable, explicitly say so.
* Multiple indicators may measure the same underlying price movement.
* **DO NOT USE MONTHLY CHARTS.**
* Use ONLY **Daily and Weekly charts** for breakout analysis.
* Prakhar's Algorithm counts as **ONE strategy**, not four separate strategies.
* For Prakhar's Algorithm, distinguish between a fresh crossover and a condition that has been true for some time.
* A stock is a **Confirmed Prakhar Breakout only when all four conditions align within the defined signal window.**
* Do not manufacture missing conditions.
* Clearly show whether the signal is Daily, Weekly, or Daily + Weekly.

---

# FINAL OBJECTIVE

The final objective is:

**FROM MY PROVIDED STOCK LIST, IDENTIFY WHICH STOCKS CURRENTLY SHOW AT LEAST ONE OF THE 8 DEFINED BREAKOUT STRATEGIES, USING ONLY DAILY AND WEEKLY CHARTS, AND SHOW THE TECHNICAL EVIDENCE FOR EACH.**

The eighth strategy is:

### PRAKHAR'S ALGORITHM

**Supertrend RED → GREEN

* OBV crosses above 8-period EMA
* RSI(14) crosses above 66
* Price confirms the upward breakout**

Analyse the Daily and Weekly versions separately and highlight **Daily + Weekly confirmation**.
