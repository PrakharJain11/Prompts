Here is a ready-to-use Gemini Pro prompt to identify stocks from your provided list whose prices have corrected and returned close to their older price levels within the last 10 weeks.

# Stock Price Recovery and Return-to-Previous-Price Scanner

## Role

Act as a quantitative stock market analyst specializing in historical price action, technical analysis, and stock screening for Indian equities listed on NSE and BSE.

## Objective

I will provide a list of stock names or ticker symbols. Analyse each stock's historical daily price data for the **last 10 weeks (approximately 50 trading sessions)** and identify stocks whose prices declined or moved away from an earlier price level and have now returned close to that level.

A stock qualifies when its latest available closing price is within **±5% of a clearly identifiable previous price level** observed during the last 10 weeks.

## Screening Methodology

### Step 1: Collect historical data

For every stock in my list, obtain reliable daily historical data covering the last 10 weeks, including:

- Date
- Open, High, Low and Close (OHLC)
- Volume
- Latest available closing price

Use adjusted historical prices where appropriate for stock splits, bonuses, and other corporate actions. Clearly state the data source and the latest date available.

### Step 2: Identify the old price level

Identify a meaningful historical reference price from the last 10 weeks. This may be:

- A previous swing high or swing low.
- A price level where the stock consolidated for several sessions.
- A previous support or resistance level.
- A price level from which the stock made a significant upward or downward move.

Do not select an arbitrary price merely because it is within 5% of the current price. Explain why the selected reference price is meaningful.

### Step 3: Check the price movement

Identify stocks that followed a pattern such as:

**Pattern A — Price fell and returned**

1. Stock traded near an identifiable old price level.
2. Its price subsequently declined meaningfully, preferably by at least 8–10% from that level.
3. It recovered and returned to within ±5% of the old price level.

**Pattern B — Price rose and returned**

1. Stock traded near an identifiable old price level.
2. Its price subsequently rose meaningfully, preferably by at least 8–10%.
3. It declined again and returned to within ±5% of the old price level.

**Pattern C — Price moved away and returned**

1. Stock moved significantly above or below a historical reference level.
2. It subsequently reversed direction.
3. Its latest closing price returned to within ±5% of that level.

The 8–10% excursion is a screening preference, not an absolute requirement. Include stocks with smaller movements in a separate section if the price pattern is otherwise meaningful.

### Step 4: Apply the ±5% rule

Calculate:

Deviation (%) = ((Latest Closing Price − Reference Price) / Reference Price) × 100

A stock meets the price-proximity condition when its deviation is between -5% and +5%, inclusive.

Also calculate:

- Reference price
- Latest closing price
- Absolute percentage deviation
- Maximum percentage decline or rise away from the reference price
- Date the stock first moved away from the reference level
- Date it returned to the ±5% range, if identifiable

### Step 5: Classify the results

Classify each qualifying stock into one of these categories:

- **Returned after correction:** Price fell below the reference level and subsequently recovered.
- **Returned after rally:** Price rose above the reference level and subsequently declined.
- **Returned after two-way volatility:** Price moved materially in either direction and later returned.
- **Near old price without meaningful excursion:** Price is within ±5%, but there is insufficient evidence of a meaningful move away. Report separately and do not treat it as a confirmed return pattern.

## Required Output

### Table 1: Main qualifying stocks

Sort the stocks by the strength and clarity of their return pattern.

| Stock | NSE Symbol | Reference Price | Latest Close | Deviation % | Maximum Excursion % | Direction | Date Moved Away | Date Returned | Days Away | Pattern |
| ----- | ---------- | --------------- | ------------ | ----------- | ------------------- | --------- | --------------- | ------------- | --------- | ------- |

Show only stocks supported by verified historical data. Use the correct NSE ticker and clearly identify the exchange.

### Table 2: Price movement summary

For each qualifying stock, provide:

- Reference price and the reason for selecting it.
- Lowest price after moving away from the reference level.
- Highest price after moving away from the reference level.
- Whether the stock has returned to the reference level from below or above.
- Whether it is currently above, below, or almost exactly at the reference price.
- Whether the stock touched the ±5% range temporarily or has remained in it for several sessions.

### Table 3: Near matches and exclusions

List stocks that almost qualify but fail one or more conditions. Explain the reason, such as:

- Current price is more than 5% away from the reference level.
- No meaningful price excursion occurred.
- The price has not yet returned.
- Historical data is incomplete or unreliable.

## Chart Validation

For each of the top qualifying stocks:

1. Plot the daily closing price over the last 10 weeks.
2. Draw a horizontal line at the selected reference price.
3. Draw upper and lower boundaries at +5% and -5% of the reference price.
4. Mark the initial move away from the level and the subsequent return.
5. Display volume beneath the price chart if the charting tool supports it.

## Data Integrity Rules

- Use actual historical prices, not estimates or assumptions.
- Do not fabricate tickers, dates, prices, or percentage calculations.
- Do not confuse a stock's 52-week high or low with a reference level inside the requested 10-week window.
- Account for stock splits, bonus issues, and other corporate actions that may distort historical comparisons.
- If data is unavailable, mark it as unavailable rather than inventing results.
- Do not claim that all supplied stocks have been analysed unless each has actually been checked.
- Include the exact start date and end date of the analysis.
- Cite reliable data sources, preferably NSE/BSE, established financial data providers, or verifiable historical-price pages.

## Final Summary

At the end, provide:

1. Total number of stocks supplied.
2. Number of stocks analysed successfully.
3. Number that satisfy the main screening criteria.
4. Number that qualify only as near matches.
5. The five clearest historical return-to-price patterns, with a short explanation of each.
6. A downloadable CSV or Excel file containing all screening results, if file creation is supported.

## Important Distinction

This is a historical price-pattern screening exercise, not a prediction of future returns. Returning to an old price level does not automatically imply support, undervaluation, or a buying opportunity.

Wait for me to provide my stock list before starting the analysis. Once I provide it, analyse the stocks individually and present evidence-backed results.

## How to use it

1. Paste the prompt into Gemini Pro or Gemini Deep Research.
2. Provide your stock list, preferably with NSE symbols.
3. Ask Gemini to verify historical prices and show the calculations rather than relying on chart-pattern descriptions alone.

My recommendation: Keep the minimum 8–10% price excursion in the screening logic. Without it, a stock that has traded sideways near the same price for 10 weeks could qualify even though it never meaningfully moved away and returned.