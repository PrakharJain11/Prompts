Absolutely. Since you want to identify **sudden/intraday volume surges from a user-provided NSE stock list**, the prompt should compare each stock's current hourly volume against its normal historical hourly volume—not simply rank stocks by absolute volume.

### Gemini Pro Prompt

# GEMINI PRO — NSE INTRADAY SUDDEN VOLUME SURGE SCANNER

## OBJECTIVE

I will provide a list of NSE stocks below.

Analyze **only the stocks from my provided list** and identify stocks showing a **sudden and abnormal volume surge**, especially during the current trading session.

The objective is to detect stocks where **current buying/trading activity is significantly higher than their normal volume**, which may indicate accumulation, institutional activity, breakout preparation, news-driven activity, or unusual market interest.

Do NOT simply select stocks having the highest absolute volume. Focus on **abnormal volume relative to the stock's own historical trading pattern**.

---

# 1. STOCK LIST — USER INPUT

I will paste my stock list below.

### START STOCK LIST

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

### END STOCK LIST

Analyze ONLY these stocks.

---

# 2. DATA FRESHNESS — VERY IMPORTANT

Use the **latest available NSE/BSE intraday data**.

First determine:

* Current trading date
* Current Indian market time
* Whether the market is currently open or closed
* Latest available trading session
* Latest available intraday candle

For the current session, use the latest available data up to the time of analysis.

If today's intraday data is unavailable, clearly state this and use the most recent session for which reliable intraday data is available.

Do NOT fabricate hourly volume data.

---

# 3. PRIMARY SCREEN — SUDDEN VOLUME SURGE

For every stock, calculate/estimate:

### A. Current Hour Volume

Volume traded during each available hourly interval:

* 9:15–10:15
* 10:15–11:15
* 11:15–12:15
* 12:15–13:15
* 13:15–14:15
* 14:15–15:15
* 15:15–15:30

Adjust the final interval according to the actual NSE trading session and available candle structure.

### B. Historical Average Hourly Volume

Compare each current hourly volume with the stock's normal volume during the **same time period** over approximately the previous **10–20 trading sessions**, wherever data is available.

Calculate:

**Hourly Volume Surge Ratio = Current Hour Volume ÷ Historical Average Volume for Same Hour**

Also calculate:

**Volume Surge % = ((Current Hour Volume / Historical Average Hourly Volume) - 1) × 100**

Example:

Historical average volume between 10:15–11:15 = 100,000 shares

Current volume = 350,000 shares

Volume Surge = 3.5×
Volume Surge = +250%

This should be considered a significant volume anomaly.

---

# 4. DETECT DIFFERENT TYPES OF VOLUME SURGES

Classify the volume activity into:

### 🔥 EXTREME SURGE

Volume ≥ 3× normal

### 🟢 STRONG SURGE

Volume ≥ 2× normal

### 🟡 MODERATE SURGE

Volume ≥ 1.5× normal

### ⚪ NORMAL

Volume < 1.5× normal

Give preference to stocks where the surge is **sudden and sustained**, rather than a single random spike.

---

# 5. DETECT SUDDEN VOLUME ACCELERATION

Look for situations such as:

### Pattern A — Sudden Spike

Normal volume:

100K → 110K → 105K → 500K

Identify this as a sudden volume event.

### Pattern B — Increasing Volume

100K → 150K → 220K → 350K → 500K

Identify this as accelerating participation.

### Pattern C — Price + Volume Confirmation

Volume increases significantly AND price simultaneously moves higher.

This is more important than volume increase alone.

### Pattern D — Volume Surge Without Price Movement

Very large volume increase but limited price movement.

Flag this separately as possible:

* Accumulation
* Distribution
* Institutional activity
* Absorption
* Large buyer/seller activity

Do NOT automatically classify this as bullish.

---

# 6. COMPARE VOLUME WITH PRICE

For every stock showing abnormal volume, analyze:

* Current price
* Today's % change
* Current day's high
* Current day's low
* Previous close
* Current volume
* Average volume
* Volume Surge %
* Volume Surge Ratio
* Whether price is above VWAP, if available
* Whether price is near today's high
* Whether price is near a breakout level

Determine whether the volume surge is:

### 🟢 Bullish Volume

High volume + rising price + strong close/near-day-high

### 🔴 Bearish Volume

High volume + falling price + weak price action

### 🟡 Accumulation/Absorption

Very high volume + relatively small price movement

### ⚪ Neutral

High volume without a clear directional signal

---

# 7. RELATIVE VOLUME SCORE

Create a **Volume Surge Score from 0–100**.

Consider:

* Current hourly volume vs historical hourly average
* Largest hourly volume surge
* Number of consecutive high-volume candles
* Daily volume vs 20-day average volume
* Price + volume confirmation
* Volume acceleration
* Position of price within today's range
* VWAP relationship
* Breakout/breakdown confirmation

Suggested interpretation:

| Score  | Interpretation             |
| ------ | -------------------------- |
| 80–100 | Extreme abnormal volume    |
| 65–79  | Strong volume activity     |
| 50–64  | Moderate volume activity   |
| 35–49  | Slightly elevated          |
| <35    | Normal/no meaningful surge |

---

# 8. HOURLY VOLUME CHART — VERY IMPORTANT

If reliable intraday data is available, **draw a separate hourly volume chart for each stock that qualifies as a significant volume-surge candidate**.

Prefer a bar chart showing:

**X-axis:** Time
**Y-axis:** Trading Volume

Example:

```text
Volume
│
│                         █
│                         █
│               █         █
│       █       █         █
│   █   █       █    █    █
│___█___█_______█____█____█____
   9:15 10:15  11:15 12:15 13:15
```

Where possible, visually distinguish:

* Normal-volume hours
* Above-average-volume hours
* Extreme-volume hours

Also show the **historical average hourly volume** as a reference line if the data source allows it.

IMPORTANT:

Do NOT create an artificial chart using estimated or fabricated numbers.

If hourly historical data is unavailable, clearly state:

> "Reliable hourly volume history is unavailable for this stock, therefore an hourly comparison chart cannot be generated."

---

# 9. RANK THE STOCKS

Create a final ranked table.

| Rank | Stock   | Symbol | Price | Day % | Current Volume | Avg Volume | Volume Ratio | Surge % | Highest Surge Hour | Score | Signal    |
| ---- | ------- | ------ | ----: | ----: | -------------: | ---------: | -----------: | ------: | ------------------ | ----: | --------- |
| 1    | Example | ABC    |  ₹XXX | +X.X% |           X.XM |       X.XM |         4.2× |   +320% | 11:15–12:15        |    92 | 🟢 Strong |
| 2    | Example | XYZ    |  ₹XXX | +X.X% |           X.XM |       X.XM |         3.1× |   +210% | 13:15–14:15        |    84 | 🟢 Strong |

Rank primarily by **abnormal volume**, not absolute volume.

---

# 10. TOP VOLUME SURGE CANDIDATES

After analyzing the complete list, provide:

## 🔥 TOP 10 VOLUME SURGE STOCKS

For each stock explain in 2–4 lines:

1. Why it was selected
2. Highest volume surge
3. When the surge occurred
4. Price reaction
5. Whether volume is sustained
6. Whether the signal appears bullish, bearish, accumulation, or neutral

---

# 11. DETECT "SMART MONEY" STYLE ACTIVITY

Where reliable data is available, check whether abnormal volume is accompanied by:

* Increasing delivery percentage
* Increasing delivery volume
* Block/bulk deals
* Institutional buying
* FII/DII activity
* Large trades
* Price holding despite heavy selling
* Price rising with increasing volume

However:

**Do NOT claim that institutional or smart-money buying occurred merely because volume increased.**

Clearly separate:

**Confirmed evidence**

from

**Possible interpretation.**

---

# 12. BREAKOUT + VOLUME CONFIRMATION

For stocks showing abnormal volume, check whether the stock is simultaneously:

* Breaking previous day's high
* Breaking recent swing high
* Breaking 20-day high
* Breaking 52-week high
* Breaking a consolidation range
* Crossing resistance
* Trading above VWAP

Give special priority to:

> **Price breakout + abnormal volume + sustained volume**

This combination should receive a higher score than volume surge alone.

---

# 13. FALSE VOLUME SURGE FILTER

Try to eliminate misleading signals caused by:

* Opening auction volatility
* One-off block trades
* Corporate announcements
* Stock split/bonus adjustments
* Extremely low liquidity
* Sudden price gaps
* Data anomalies
* Illiquid stocks
* One isolated candle without continuation

If a stock has a large volume spike but no meaningful confirmation, mark it:

**"Volume spike — confirmation required."**

---

# 14. FINAL CLASSIFICATION

Classify every shortlisted stock into one of these categories:

### 🟢 A — High-Quality Bullish Volume

Abnormal volume + rising price + breakout/strong price action

### 🟢 B — Bullish Volume Acceleration

Increasing volume + positive price momentum

### 🟡 C — Accumulation Candidate

Very high volume + limited downside/sideways price movement

### 🔴 D — Bearish Volume

Abnormal volume + significant price decline

### 🟠 E — Volume Spike — No Confirmation

Abnormal volume but unclear direction

---

# 15. FINAL OUTPUT STRUCTURE

Return the report in this order:

## 1. Market/Data Status

* Trading date
* Latest data timestamp
* Market open/closed
* Data source
* Number of stocks analyzed

## 2. 🔥 Top Volume Surge Stocks

Ranked table.

## 3. 📊 Hourly Volume Analysis

For each significant candidate:

**Stock Name — SYMBOL**

* Current price
* Day change
* Volume
* Average volume
* Volume ratio
* Maximum hourly surge
* Time of surge
* Price reaction
* Volume classification

Then show the hourly volume chart.

## 4. 🚀 Volume + Price Breakout Candidates

Identify stocks where abnormal volume is supporting a price breakout.

## 5. 🐋 Possible Accumulation / Institutional Activity

Only where evidence supports the conclusion.

## 6. ⚠️ Volume Spike Without Confirmation

Stocks that experienced unusual volume but don't yet have convincing price confirmation.

## 7. 🏆 Final Ranking

Rank the best opportunities based on:

**Volume abnormality + volume acceleration + price confirmation + breakout + sustainability**

---

# 16. IMPORTANT RULES

1. Analyze ONLY the stocks I provide.
2. Do not add random stocks from outside my list.
3. Do not rely only on daily volume.
4. Give maximum importance to **intraday hourly volume behavior**.
5. Compare volume with the stock's own historical volume.
6. Prefer same-time-of-day historical comparison.
7. Do not treat high absolute volume as abnormal volume.
8. Do not fabricate missing hourly data.
9. Clearly identify the data timestamp.
10. Clearly distinguish facts from interpretation.
11. Do not call volume automatically "smart money".
12. Consider both price and volume together.
13. Give higher priority to sustained volume expansion.
14. Identify the exact hour in which the abnormal volume started.
15. Highlight stocks where volume surge is accompanied by a breakout.
16. If possible, generate a separate hourly volume chart for every significant candidate.
17. If the market is currently open, use the latest available intraday data rather than waiting for the market to close.
18. If data quality is insufficient, explicitly say so rather than guessing.

## PRIMARY OBJECTIVE

The final result should answer one simple question:

> **"From my provided stock list, which stocks are experiencing an unusual/sudden increase in trading volume RIGHT NOW, and is that volume supporting bullish price action?"**

Focus on **abnormal volume, timing of the surge, volume acceleration, price confirmation and breakout potential**, rather than simply ranking stocks by total traded volume.

This version is particularly useful for your **breakout-screening workflow** because it separates **"high volume"** from **"abnormally high volume"** and then adds the crucial **price + volume confirmation** layer.
