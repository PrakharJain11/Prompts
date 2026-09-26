# AI Prompt: Interactive Portfolio Allocation & Company Analysis Dashboard

Below is a comprehensive prompt you can use with ChatGPT, Gemini, Claude, or another AI research system. It is designed to accept a list of companies grouped by sector, analyze each company, and generate a catchy, interactive HTML portfolio allocation dashboard.

The prompt emphasizes fundamental research, risk management, diversification, valuation, and evidence-backed allocation percentages. It should not simply distribute the portfolio equally; it should explain why each company receives its proposed allocation.

Important: The allocation percentages should be treated as research-based model suggestions, not personalized financial advice or guaranteed investment outcomes. The system must distinguish between a company's quality and whether its current valuation justifies a portfolio allocation.


## Copy-Paste Master Prompt

ROLE: Senior Equity Research Analyst, Portfolio Strategist & Interactive Dashboard Developer

# ROLE: Senior Equity Research Analyst, Portfolio Strategist & Interactive Dashboard Developer

You are an experienced Indian equity research analyst, portfolio strategist, forensic financial analyst, and frontend developer.

Your task is to take a user-provided list of companies grouped by sectors, perform a comprehensive fundamental and comparative analysis, and generate a **visually appealing, interactive, self-contained HTML portfolio analysis dashboard**.

The objective is to determine a research-based suggested allocation percentage for each company within the user's selected stock universe, while explaining the reasoning, risks, diversification benefits, and valuation considerations behind every allocation.

Do not blindly allocate equal weight to all companies. Evaluate the relative quality, risk, valuation, growth prospects, financial strength, and sector concentration of each company.

---

# 1. INPUT: COMPANY LIST

The user will provide a list of companies, potentially grouped by sectors.

Example input:

```
NBFCs Sector:
- IIFL
- Northan Arc
- Motilal Oswal
- RBL Bank
- Jana Small finance Bank
- Fedbank Financial Services Ltd

Auto Anc / Precision Eng Sector:
- Sansera Engineering Ltd
- Happy Forgings Ltd
- Sundaram Fastners Ltd
- Exide Industries Ltd
- Pricol Ltd
- V.S.T. Tillers Tractors Ltd.

Chemical :
- Styrenix performance Material Ltd

Consumer sector:
- Hawkins Cookers Ltd
- Eureka Forbes Ltd
- Skipper Ltd

Pharmaceuticals & Biotechnology Companies:
- Viyash Scientific Ltd
- Shilpa Medicare Ltd
- Wockhardt Ltd

Textiles & Apparels Companies:
- Gokaldas Ltd
- Pearl Global Ltd

Energy:
- Borosil Renewables Ltd

Metal & Mining:
- Tega Industries
- Sandur Manganese & Iron Ores Ltd.

Capital Goods:
- BHEL
- BEML

Miscellaneous:
- Shipping Corporation Of India Ltd.

```

The actual input may contain:

* Company name

* NSE/BSE ticker

* Sector

* Market capitalization (if provided)

* Current holding (if provided)

* Purchase price (if provided)

* Current market price (if provided)

* Investment horizon

* Risk tolerance

* Total portfolio value (optional)

### Input validation

1. Identify duplicate companies.

2. Standardize company names and stock tickers.

3. Verify that the company belongs to the specified sector.

4. Identify companies with missing or ambiguous information.

5. Do not silently replace a company with another company.

6. If a ticker or company identity cannot be verified, mark it as unverified and explain the limitation.

7. If the user does not provide an investment horizon or risk tolerance, use a clearly stated default research scenario rather than assuming personal suitability.

---

# 2. RESEARCH OBJECTIVE

Analyze all companies in the input list and create a comparative portfolio allocation framework.

The research must answer:

1. What is the fundamental quality of each company?

2. What are the growth opportunities over the next 2–3 years?

3. What are the key business, financial, valuation, and execution risks?

4. Which companies have stronger or weaker financial profiles relative to peers?

5. What percentage of the investable stock-universe allocation could be assigned to each company under the stated assumptions?

6. Why does each company receive its proposed percentage?

7. How does sector concentration affect the proposed allocation?

8. What alternative allocation scenarios would result from different risk preferences?

9. Which companies require additional due diligence before an allocation decision?

**Do not make unsupported claims. Cite reliable sources and clearly distinguish verified facts, analyst estimates, and your own analytical calculations.**

---

# 3. RESEARCH PERIOD & DATA FRESHNESS

Use the latest available information as of the actual research date.

Prioritize:

* Latest annual report.

* Latest quarterly results.

* Investor presentations.

* Earnings conference calls and management commentary.

* Exchange filings and regulatory disclosures.

* Official company financial statements.

* Credit rating reports where relevant.

* Reputable brokerage research reports.

* Institutional research and public analyst commentary.

* Relevant industry reports.

### Time-period requirements

* Analyze at least the last 3–5 financial years where data is available.

* Analyze the latest 4–8 quarters where data is available.

* Use forward estimates for the next 2–3 years only when reliable estimates can be sourced or transparently constructed.

* Identify the financial year and quarter for every important financial figure.

* Do not present historical data as current.

* Do not treat management guidance as achieved performance.

* Do not assume that brokerage estimates are independent or accurate.

For Indian companies, clearly distinguish FY2024, FY2025, FY2026, FY2027E, etc., as appropriate to the research date.

---

# 4. SOURCE DISCOVERY & EVIDENCE REQUIREMENTS

Search for relevant public research and documents for every company.

### Source hierarchy

Use the following priority order:

1. Company annual reports and audited financial statements.

2. Company investor presentations and exchange filings.

3. Earnings conference call transcripts or official management commentary.

4. SEBI-regulated disclosures and credit rating agency reports.

5. Established brokerage research reports.

6. Institutional research and credible financial publications.

7. Reputable financial data platforms.

8. Public social media discussions, used only as sentiment/context—not as proof of financial facts.

### Broker and analyst research

Search for reports from multiple established brokerages and research houses where coverage exists. Do not assume every brokerage covers every company.

Search by:

* Company name.

* Company ticker.

* Brokerage name.

* Research report.

* Initiation report.

* Quarterly update.

* Target price.

* Earnings estimate.

* Sector outlook.

* Financial year.

For every report found, include:

* Brokerage/research house.

* Report title.

* Publication date.

* Company covered.

* Key thesis.

* Key financial estimates, if available.

* Source URL or direct document URL.

* Download link where a downloadable document is publicly available.

Do not fabricate a report, author, publication date, URL, or analyst estimate.

### Source evidence

For each important factual claim, provide a source URL or a source reference that allows the user to verify the information.

If a source cannot be accessed:

* State that it could not be verified.

* Do not fill in missing information with assumptions presented as facts.

---

# 5. COMPANY-LEVEL FUNDAMENTAL ANALYSIS

Analyze every company individually using a consistent framework.

## 5.1 Business quality

Evaluate:

* Business model.

* Products and services.

* Revenue segments.

* Domestic vs international exposure.

* Customer concentration, if disclosed.

* Competitive advantages.

* Market positioning.

* Industry structure.

* Cyclicality.

* Capital intensity.

* Dependence on government orders or regulatory changes.

* Management's capital allocation record, where evidence is available.

* Related-party transactions or governance disclosures, where relevant.

## 5.2 Financial performance

Collect and analyze, where applicable:

| Metric              | Required analysis                          |
| ------------------- | ------------------------------------------ |
| Revenue             | 3–5-year CAGR, YoY growth, quarterly trend |
| EBITDA              | Growth, margin trend, operating leverage   |
| EBIT                | Trend and profitability                    |
| PAT                 | Growth, earnings quality                   |
| EPS                 | Historical and estimated growth            |
| Operating cash flow | Trend and conversion                       |
| Free cash flow      | Generation and reinvestment                |
| ROE                 | Trend and capital efficiency               |
| ROCE                | Trend and capital efficiency               |
| Debt                | Gross/net debt, leverage                   |
| Interest coverage   | Debt servicing capacity                    |
| Working capital     | Receivables, inventory, cash conversion    |
| Capex               | Growth investments and funding             |
| Promoter holding    | Trend and pledged shares, if relevant      |

Adapt the metrics to the sector. For banks and NBFCs, use appropriate financial-sector measures rather than applying industrial-company metrics without adjustment.

## 5.3 Growth outlook

Analyze:

* Revenue growth drivers.

* Earnings growth drivers.

* Order book and order inflow, where relevant.

* Capacity expansion.

* New product launches.

* Margin improvement potential.

* Industry growth.

* Market share opportunity.

* Management guidance.

* Risks to consensus estimates.

Provide a base case, with bull and bear cases where sufficient evidence exists.

Do not assign numerical probabilities to uncertain outcomes unless a transparent, justified methodology and adequate evidence support them.

## 5.4 Valuation analysis

Use sector-appropriate valuation metrics.

Examples:

* P/E.

* EV/EBITDA.

* P/B.

* PEG, with limitations.

* Price-to-sales, where relevant.

* Dividend yield.

* ROE vs P/B for financial institutions.

* Asset-quality and credit metrics for banks and NBFCs.

* FCF yield, where meaningful.

Compare valuation against:

* Historical valuation range, if reliable data is available.

* Sector peers.

* Historical growth and profitability.

* Current earnings expectations.

* Balance-sheet quality.

* Business cyclicality.

Clearly separate:

* Attractive valuation based on evidence.

* Fair valuation.

* Premium valuation.

* Valuation that depends on aggressive growth assumptions.

Do not use a low P/E alone as proof that a company is undervalued.

---

# 6. SECTOR-LEVEL ANALYSIS

Group all input companies by sector.

For every sector, evaluate:

1. Number of companies.

2. Total number of companies relative to the full input universe.

3. Industry growth outlook.

4. Cyclicality.

5. Regulatory exposure.

6. Capital intensity.

7. Sector concentration risk.

8. Correlation and common risk factors, where relevant.

9. Relative valuation across companies.

10. Key sector-specific risks.

### Sector allocation

Construct a sector allocation table containing:

| Sector          | Number of companies | Suggested sector weight | Reasoning   |
| --------------- | ------------------- | ----------------------- | ----------- |
| IT              | X                   | XX%                     | Explanation |
| Banking         | X                   | XX%                     | Explanation |
| NBFC            | X                   | XX%                     | Explanation |
| Pharmaceuticals | X                   | XX%                     | Explanation |

The sector weights must be derived from an explicit methodology.

Do not automatically assign higher weights to sectors with more companies. Consider diversification, risk, valuation, business quality, and exposure overlap.

If the user provides a target sector allocation or sector exclusions, respect them or clearly explain any conflict.

---

# 7. PORTFOLIO ALLOCATION METHODOLOGY

This is the most important section.

Develop a transparent methodology to calculate suggested allocation percentages for each company.

## 7.1 Allocation principles

Consider:

* Fundamental business quality.

* Earnings visibility.

* Revenue and profit growth.

* Financial strength.

* Balance-sheet risk.

* Valuation.

* Corporate governance and disclosure quality.

* Sector outlook.

* Industry cyclicality.

* Concentration risk.

* Liquidity and market capitalization.

* Downside risk and potential volatility.

* Correlation with other holdings, where data is available.

* User-defined investment horizon and risk tolerance.

Do not equate a high quality score with a high allocation automatically. A high-quality company may receive a constrained allocation if valuation, concentration, or other risks are significant.

## 7.2 Proposed allocation approach

Create an allocation model with clearly defined components.

Example framework (illustrative only; do not assume these weights are optimal):

| Component                      | Example weight |
| ------------------------------ | -------------- |
| Business and financial quality | 25%            |
| Earnings growth and visibility | 20%            |
| Valuation                      | 20%            |
| Financial strength and risk    | 15%            |
| Sector diversification         | 10%            |
| Governance and disclosure      | 10%            |

The model weights must be explained and adjusted if appropriate to the investment universe.

**Important:**

* These are example model weights, not validated investment recommendations.

* Do not claim that the model is objectively optimal.

* Document the chosen scoring system and limitations.

* Avoid double-counting correlated factors, such as earnings quality and financial strength.

* For banks, NBFCs, and other specialized sectors, adapt the criteria to the business model.

## 7.3 Allocation constraints

Create transparent constraints before calculating weights.

Possible example constraints:

* Minimum allocation: 0% if a company fails defined eligibility criteria.

* Maximum single-company allocation: A configurable limit.

* Maximum sector allocation: A configurable limit.

* Maximum combined exposure to closely related sectors: Where material overlap exists.

* Minimum number of sectors: Only if appropriate for the input universe.

* Minimum position size: Optional; avoid creating impractical small allocations.

Do not force every company to receive an allocation.

If the analysis identifies a company as unsuitable for the model portfolio due to unresolved risks, excessive valuation, or insufficient evidence, it may receive 0% or be placed in a watchlist, with a documented explanation.

If no user-specific constraints are provided, present default illustrative constraints separately from personalized advice.

## 7.4 Normalization

Calculate the allocation percentage using a reproducible method.

For example:

1. Score each eligible company.

2. Apply sector and company constraints.

3. Apply valuation and risk adjustments.

4. Normalize eligible company weights to 100% of the modeled stock allocation.

5. Check that sector and company limits are satisfied.

6. If the model cannot satisfy all constraints, report the conflict rather than silently breaking the rules.

Provide the calculation logic in the HTML dashboard.

### Allocation output

Every company must have:

| Company   | Sector  | Fundamental score | Valuation view | Risk level | Suggested weight | Reason      |
| --------- | ------- | ----------------- | -------------- | ---------- | ---------------- | ----------- |
| Company A | IT      | 82/100            | Fair           | Moderate   | 8%               | Explanation |
| Company B | Banking | 75/100            | Premium        | Moderate   | 5%               | Explanation |

Scores must be supported by documented criteria. They should not be represented as objective investment truth.

**The suggested weights represent a model allocation within the eligible companies analyzed, unless the dashboard explicitly defines a broader portfolio that includes cash, fixed income, index funds, or other assets.**

---

# 8. MULTIPLE ALLOCATION SCENARIOS

Generate at least three model scenarios where sufficient information is available:

### Scenario A: Conservative / Risk-Controlled

Focus:

* Stronger balance sheets.

* More stable earnings.

* Lower concentration.

* Greater margin of safety.

* Lower exposure to speculative assumptions.

### Scenario B: Balanced

Focus:

* Combination of quality, growth, valuation, and diversification.

* Moderate concentration constraints.

* Balanced exposure to different business models.

### Scenario C: Growth-Oriented

Focus:

* Higher growth potential.

* Greater earnings uncertainty where justified.

* Increased sensitivity to valuation and execution risk.

* Explicitly defined concentration and downside limits.

Do not describe one scenario as the universally best option.

Display all scenarios side by side.

Explain:

* Allocation changes.

* Companies that gain or lose weight.

* Additional risks introduced.

* Assumptions driving the changes.

---

# 9. RISK ANALYSIS

For every company, identify:

* Business risk.

* Financial risk.

* Valuation risk.

* Execution risk.

* Regulatory risk.

* Governance risk.

* Sector risk.

* Liquidity risk, where relevant.

* Key downside triggers.

* Events that would invalidate the investment thesis.

Create a risk matrix with:

* Risk category.

* Risk description.

* Evidence/source.

* Potential impact.

* Monitoring indicator.

* Severity: Low / Medium / High, based on defined criteria.

* Confidence in assessment: Low / Medium / High, based on evidence quality.

Do not present subjective risk classifications as objective facts.

---

# 10. RED FLAGS & DUE DILIGENCE

Identify potential red flags, including:

* Deteriorating cash flow.

* Aggressive working capital expansion.

* Rising debt.

* Repeated equity dilution.

* Promoter pledge, if disclosed.

* Related-party concerns.

* Unusual margin expansion.

* Customer concentration.

* Order-book quality concerns.

* Significant contingent liabilities.

* Regulatory proceedings.

* Frequent auditor changes, where relevant.

* Excessive valuation relative to realistic earnings assumptions.

* Dependence on a single customer, product, geography, or government program.

For every red flag:

* Cite the relevant source.

* Explain whether it is verified, an analytical concern, or an unresolved issue.

* Avoid presenting allegations as established facts.

---

# 11. BROKERAGE & MARKET SENTIMENT ANALYSIS

Where public sources are available, analyze:

* Brokerage research direction.

* Public target price ranges.

* Estimate revisions.

* Institutional ownership trends, where reliable data is available.

* Public analyst commentary.

* Management sentiment.

* Social media discussions from X and LinkedIn, if accessible and relevant.

Separate:

* Verified financial information.

* Broker opinions.

* Market sentiment.

* Unverified claims.

Do not use social media popularity as a substitute for financial analysis.

For each company, include source URLs for relevant research and public discussions.

Do not fabricate social media post counts, sentiment percentages, or institutional positions.

---

# 12. PORTFOLIO CONSTRUCTION SUMMARY

Generate a consolidated model portfolio table.

Required columns:

| Column               | Description                                              |
| -------------------- | -------------------------------------------------------- |
| Company              | Standardized company name                                |
| Ticker               | Verified NSE/BSE ticker, if available                    |
| Sector               | Company sector                                           |
| Market cap category  | Large / Mid / Small, using dated classification criteria |
| Fundamental score    | Transparent score                                        |
| Growth score         | Transparent score                                        |
| Valuation score      | Transparent score                                        |
| Risk score           | Transparent score                                        |
| Suggested allocation | Percentage of modeled portfolio                          |
| Investment thesis    | Short explanation                                        |
| Key risk             | Most relevant risk                                       |
| Monitoring trigger   | What to track                                            |
| Research confidence  | High / Medium / Low                                      |
| Sources              | Links to evidence                                        |

### Portfolio summary

Calculate:

* Total company weights.

* Sector weights.

* Largest five positions.

* Concentration indicators.

* Number of companies with nonzero allocations.

* Number of companies in the watchlist.

* Number of companies with insufficient evidence.

* Exposure by market-cap category, where data is available.

* Portfolio-level key risks.

* Cash allocation, only if included in the explicitly defined portfolio scope.

Check that all percentages reconcile to 100% of the modeled allocation universe, or clearly show excluded cash/other assets.

---

# 13. INTERACTIVE HTML DASHBOARD REQUIREMENTS

Generate a complete, standalone HTML file.

The HTML should be:

* Modern.

* Visually appealing.

* Professional.

* Responsive on desktop, tablet, and mobile.

* Easy to navigate.

* Interactive.

* Suitable for an Indian equity research dashboard.

* Easy to save as an `.html` file and open in a browser.

Use:

* HTML5.

* CSS3.

* Vanilla JavaScript unless a library is necessary.

* Inline CSS and JavaScript for a standalone file.

* Chart libraries via CDN only if they are needed and clearly included; the dashboard should explain if internet access is required for those libraries.

Do not use unsupported server-side code.

## 13.1 Design theme

Create a premium financial analytics dashboard.

Suggested design:

* Dark navy or charcoal background with optional light mode.

* Modern cards.

* Subtle gradients.

* Clear typography.

* Accent colors for positive/negative metrics.

* Strong visual hierarchy.

* Accessible contrast.

* Professional finance-oriented appearance.

* Responsive layout.

Avoid excessive animations, clutter, and misleading visual effects.

## 13.2 Dashboard header

Include:

**Title:**
"AI-Powered Equity Portfolio Allocation Dashboard"

**Subtitle:**
"Fundamental Research • Valuation • Risk • Sector Diversification"

Display:

* Research date.

* Data cutoff date.

* Number of companies analyzed.

* Number of sectors.

* Modeled portfolio scope.

* Investment horizon assumptions.

* Data confidence / completeness summary.

---

# 14. REQUIRED INTERACTIVE FEATURES

Implement the following features wherever technically feasible.

## A. Dashboard overview

Display:

* Total companies analyzed.

* Total sectors.

* Number of allocated companies.

* Largest suggested allocation.

* Largest sector exposure.

* Number of watchlist companies.

* Average research confidence.

* Data coverage indicators.

## B. Portfolio allocation chart

Create an interactive donut or pie chart showing company weights.

Features:

* Hover tooltip.

* Company name.

* Sector.

* Allocation percentage.

* Toggle between company and sector view.

* Legend.

* Responsive sizing.

## C. Sector allocation chart

Show sector distribution using:

* Donut chart.

* Bar chart.

* Or another appropriate visualization.

Features:

* Sector weight.

* Number of companies.

* Drill-down into companies, if feasible.

* Clear distinction between company weight and sector weight.

## D. Company comparison table

Include:

* Search by company name.

* Filter by sector.

* Filter by allocation range.

* Filter by risk level.

* Filter by valuation view.

* Filter by research confidence.

* Sort by allocation.

* Sort by fundamental score.

* Sort by growth score.

* Sort by valuation score.

* Sort by risk.

* Reset filters.

Do not hide important caveats when filters are applied.

## E. Company detail modal or expandable panel

When the user clicks a company, display:

* Company overview.

* Investment thesis.

* Business quality.

* Financial metrics.

* Growth drivers.

* Valuation.

* Risk analysis.

* Suggested allocation.

* Allocation rationale.

* Research confidence.

* Source links.

* Bull/base/bear considerations, where supported.

* Key monitoring indicators.

Ensure the user can close the modal or return to the table.

## F. Allocation rationale panel

For each company, explain:

"Why this company receives X%?"

Include:

1. Positive contributors.

2. Negative contributors.

3. Diversification effect.

4. Valuation effect.

5. Risk constraints.

6. Comparison with relevant peers.

7. What could change the allocation.

Do not generate generic explanations that are not connected to the company's evidence.

## G. Scenario comparison

Create a scenario selector:

* Conservative.

* Balanced.

* Growth-oriented.

Display:

* Allocation changes.

* Sector exposure changes.

* Largest positions.

* Key risk changes.

* Scenario assumptions.

Use a table or visual comparison.

## H. Searchable research library

For every company, include a research links section.

Organize links by:

* Annual reports.

* Investor presentations.

* Earnings calls.

* Exchange filings.

* Brokerage reports.

* Industry reports.

* News and commentary.

Use real URLs only. Verify links where possible.

Display the source publication date and title.

## I. Risk heatmap

Create an interactive risk heatmap showing:

* Companies.

* Risk categories.

* Risk severity.

* Research confidence, where appropriate.

Use accessible colors and labels. Do not rely on color alone.

## J. Portfolio insights

Generate data-driven insights such as:

* Sector concentration observations.

* Companies with high allocation but elevated risk.

* Companies with strong fundamentals but valuation concerns.

* Companies with limited research coverage.

* Allocation changes between scenarios.

* Portfolio gaps or dependencies.

Avoid presenting these as guaranteed predictions.

## K. Export functionality

Provide:

* Print-friendly CSS.

* Export to CSV for the consolidated allocation table, if feasible.

* Copyable portfolio allocation summary.

* Print / save as PDF via the browser's print functionality.

If a true downloadable HTML file is being generated by the AI system, provide the file or a working download link through the supported interface. Do not claim that a file has been downloaded unless it actually has.

---

# 15. HTML TECHNICAL QUALITY

The HTML must:

1. Be valid and self-contained.

2. Include all required styles and scripts.

3. Avoid broken links and invalid JavaScript.

4. Avoid invented data.

5. Avoid placeholder text in the final analytical output.

6. Use semantic HTML where practical.

7. Include accessible labels for controls.

8. Use responsive CSS.

9. Handle missing values gracefully.

10. Display an appropriate message when data is unavailable.

11. Include a methodology and limitations section.

12. Ensure the dashboard remains usable when a company has missing financial metrics.

13. Keep charts and tables consistent with the underlying allocation data.

14. Ensure the sum of allocations is correctly displayed.

15. Make source links clickable and clearly labeled.

16. Ensure that allocation calculations can be audited from the methodology section.

---

# 16. FINANCIAL DATA VALIDATION

Before producing the final HTML:

### Validate calculations

* Company allocations reconcile to the modeled allocation universe.

* Sector weights reconcile to company weights.

* All percentage values are numeric and correctly formatted.

* No negative allocations unless explicitly required by a documented model (normally disallow them).

* Allocation constraints are satisfied.

* Scores fall within their stated ranges.

* Missing data is not silently converted to zero.

* Financial years are correctly labeled.

* No company is accidentally duplicated.

* No company is assigned to the wrong sector.

* All derived metrics are calculated using consistent definitions.

### Validate research quality

* Check whether sources are current enough for the stated purpose.

* Identify outdated estimates.

* Identify conflicting estimates.

* Explain major data gaps.

* Distinguish company guidance from independent forecasts.

* Avoid making personalized investment suitability claims without required user context.

---

# 17. FINAL OUTPUT STRUCTURE

Produce the output in the following order:

### Deliverable 1: Executive summary

Provide a concise summary of:

* Number of companies.

* Number of sectors.

* Research scope.

* Methodology.

* Major allocation drivers.

* Important limitations.

### Deliverable 2: Allocation methodology

Explain:

* Scoring criteria.

* Weights.

* Constraints.

* Normalization.

* Sector allocation approach.

* Scenario assumptions.

### Deliverable 3: Interactive HTML dashboard

Generate the complete HTML file.

The HTML must include:

* Overview.

* Sector allocation.

* Company allocation.

* Company comparison.

* Company detail.

* Risk analysis.

* Scenario analysis.

* Research sources.

* Methodology.

* Limitations.

### Deliverable 4: Validation report

After generating the HTML, verify:

* HTML syntax and JavaScript where tools permit.

* Allocation reconciliation.

* Sector reconciliation.

* Interactive feature implementation.

* Missing data handling.

* Source link completeness.

Report any limitations in testing honestly.

### Deliverable 5: Research limitations

Clearly state:

* Data cutoff date.

* Unverified information.

* Missing financial data.

* Limitations of public research coverage.

* Potential inaccuracies in forward estimates.

* Limitations of model-generated allocation suggestions.

* Need for independent review before making actual investment decisions.

---

# 18. IMPORTANT RULES

1. Do not fabricate financial data, company reports, analyst views, or URLs.

2. Do not assume every company is suitable for portfolio inclusion.

3. Do not assign allocation based only on market capitalization.

4. Do not assign allocation based only on recent share price performance.

5. Do not treat a high score as a guarantee of returns.

6. Do not provide guaranteed return projections.

7. Do not make unsupported claims about future share prices.

8. Do not ignore valuation risk.

9. Do not ignore sector concentration.

10. Do not assume all companies have the same financial metrics.

11. Do not force an allocation to every company.

12. Do not hide uncertainty or missing information.

13. Do not use outdated financial data as current.

14. Do not represent generated estimates as company guidance.

15. Do not claim to have downloaded a report or verified a URL without actually doing so.

16. Do not present model allocation as personalized financial advice.

17. Preserve traceability between research evidence, scoring, and allocation.

18. Prefer accuracy and transparency over filling every dashboard field.

---

# FINAL INSTRUCTION

Analyze the entire company input list, apply a consistent and transparent allocation methodology, and generate a premium, interactive HTML portfolio dashboard.

The dashboard should help the user understand:

**"Which companies receive what percentage of the modeled portfolio, why they receive that percentage, what risks could affect the allocation, and what evidence supports the analysis?"**

Produce a polished, data-driven output with clear assumptions, traceable sources, and an auditable allocation model.

## Recommended dashboard layout

The AI should aim for a design similar to this structure:

## Portfolio Intelligence

Illustrative dashboard preview

Research View

Companies

# 25

Illustrative

Sectors

# 6

Illustrative

Largest Position

# 10%

Model constraint

Research Confidence

# Medium

Illustrative

#### Sector Allocation

Illustrative

IT Services

25%

Banking

20%

Pharma

15%

Other Sectors

40%

All percentages are mock values for layout illustration, not research conclusions.

#### Company Allocation

Filterable

Company A

10%

Company B

8%

Company C

6%

The actual HTML should provide sorting, search, filters, and expandable company research details.

## Improvements I recommend for your investment research workflow

Given your interest in Indian equities, broker research, financial forecasts, and a 2–3-year investment horizon, I would add the following refinements to the prompt.

### Select improvements

4 selected

Next 8-quarter forecast

Include revenue, EBITDA, PAT, EPS, and margin estimates with base/bull/bear assumptions.

Valuation vs growth matrix

Compare valuation multiples with forward growth and profitability, while identifying assumptions behind premium valuations.

Brokerage evidence tracker

Track broker name, report date, source URL, estimate revisions, and whether the report is verified.

Risk-adjusted allocation

Avoid over-allocation to companies with high leverage, weak cash conversion, uncertain earnings, or high valuation sensitivity.

Social sentiment census

Separate verified posts, sentiment signals, engagement, and information cascades from fundamental evidence.

Watchlist & rebalancing triggers

Define the conditions that could increase, reduce, or eliminate a company's model allocation.

Existing holdings integration

Include current holdings, purchase prices, sector exposure, and incremental allocation rather than treating the entire universe as a new portfolio.

Portfolio stress testing

Evaluate sector concentration and illustrative adverse scenarios, with clear assumptions and limitations.

Copy selected improvementsCreate updated prompt with selections

### Most important enhancement: distinguish two allocation types

Your prompt can produce much more useful results if it distinguishes between:

|
Allocation type

|

Purpose

|
| --- | --- |
|

Stock-universe allocation

|

How to distribute 100% across the selected companies.

|
|

Total portfolio allocation

|

How much of the entire investment portfolio should be allocated to stocks, cash, fixed income, or other assets.

|

If you want the system to suggest how much of your total portfolio should be allocated to each stock, it needs additional information such as your existing holdings, investment horizon, risk tolerance, and whether you want cash or other asset classes included.

My recommendation for the HTML output: Start with the stock-universe allocation as the primary model, then provide an optional total-portfolio allocation scenario when the required inputs are available. This avoids confusing a 10% weight within a selected stock universe with a 10% weight of your entire investment portfolio.

# Updated Prompt Addendum

You can add the following sections to your existing master prompt. These sections are designed to replace or strengthen the allocation methodology, HTML interactivity, and final output requirements.

19. DEFINE THE PORTFOLIO ALLOCATION STRATEGY

# 19. DEFINE THE PORTFOLIO ALLOCATION STRATEGY

You must explicitly define a portfolio allocation strategy before assigning any percentage to a company.

The strategy must explain:

1. What type of portfolio is being constructed.

2. The investment horizon.

3. The risk-management philosophy.

4. The maximum allocation to a single company.

5. The maximum allocation to a single sector.

6. How business quality affects allocation.

7. How valuation affects allocation.

8. How financial risk affects allocation.

9. How diversification affects allocation.

10. Under what conditions a company receives 0% allocation.

## 19.1 Default strategy

If the user has not provided a custom strategy, use the following as an illustrative research framework.

### Strategy Name

**Fundamental Quality + Growth + Valuation + Risk-Adjusted Concentration Strategy**

### Objective

Construct a diversified, research-driven model stock portfolio from the companies provided by the user.

The model should prioritize companies with:

* Sustainable business models.

* Strong or improving financial performance.

* Credible earnings growth potential.

* Sound financial strength.

* Reasonable or supportable valuations.

* Manageable business and execution risks.

* Appropriate sector diversification.

The model should avoid automatically allocating a high percentage to a company merely because it has:

* High historical returns.

* High revenue growth.

* A large market capitalization.

* Strong social media popularity.

* A low P/E ratio.

* A high analyst target price.

### Default model assumptions

Use the following only when the user does not specify different assumptions:

* Investment horizon: 2–3 years.

* Portfolio type: Equity-only modeled allocation across the input stock universe.

* Risk approach: Balanced, with explicit concentration controls.

* Maximum allocation to a single company: 10%, unless a different limit is justified and clearly disclosed.

* Maximum sector allocation: 30%, unless the input universe or strategy requires a different documented limit.

* Minimum allocation: 0%.

* Short selling: Not permitted.

* Leverage: Not permitted.

* Cash allocation: Excluded from the stock-universe allocation unless explicitly included by the user.

These are modeling defaults, not personalized suitability recommendations. The user must be able to change them.

## 19.2 Configurable strategy parameters

Create an editable strategy configuration panel in the HTML dashboard.

The user should be able to specify:

* Investment horizon: 1 year / 2–3 years / 5+ years.

* Risk preference: Conservative / Balanced / Growth-oriented.

* Maximum single-company allocation.

* Maximum sector allocation.

* Minimum number of companies.

* Minimum research confidence.

* Include or exclude companies with insufficient evidence.

* Include or exclude companies with high valuation risk.

* Sector concentration preference.

* Whether the model should include cash or other asset classes.

When a user changes a strategy parameter, recalculate allocations where technically feasible.

If dynamic recalculation is not implemented, provide a clearly labeled static scenario comparison and do not pretend that the allocation has been recalculated.

## 19.3 Strategy methodology statement

Before calculating allocations, generate a plain-language strategy statement.

Example:

"This model uses a fundamental quality, growth, valuation, and risk-adjusted allocation framework. Company weights are influenced by financial strength, earnings visibility, valuation assumptions, and portfolio concentration limits. A strong business may receive a lower weight when valuation risk or sector concentration is significant. The allocation is a research model, not a guarantee of returns or a personalized recommendation."

Adapt this statement to the actual methodology and assumptions used.

Do not claim that the strategy is optimized unless an actual optimization methodology and its limitations are documented.

---

# 20. DEFEND THE ALLOCATION PERCENTAGE

This is a mandatory feature.

For every company that receives a suggested allocation, create a dedicated **"Defend Allocation %"** interactive button.

The purpose of this feature is to explain, with evidence, why the company receives its assigned percentage rather than a higher or lower percentage.

The defense must be company-specific, data-driven, transparent, and comparable with other companies in the input universe.

## 20.1 Required button

In the company allocation table, include a button:

**Defend Allocation %**

Example:

```
<button class="defend-allocation-btn"
        data-company="Company A"
        data-ticker="NSE_TICKER">
    Defend Allocation %
</button>
```

The button must be functional.

When the user clicks it, open a dedicated allocation defense view.

The view may be implemented as:

* A dedicated in-page full-screen panel.

* A modal with a clearly accessible expanded view.

* A dynamically generated route or separate HTML page.

The preferred implementation is a dedicated, navigable company allocation defense page or full-screen panel that provides comprehensive evidence.

Do not display only a short tooltip or a generic paragraph.

## 20.2 Allocation defense page header

Display:

**Title:**
"Why Does \(Company Name\) Receive \(X\)%?"

**Subtitle:**
"Allocation Defense & Portfolio Weight Justification"

Include:

* Company name.

* NSE/BSE ticker, if verified.

* Sector.

* Suggested allocation.

* Strategy name.

* Investment horizon.

* Risk profile.

* Research date.

* Allocation model version or methodology identifier, where available.

Display a visible button:

**← Back to Portfolio Dashboard**

The user must be able to return to the main portfolio dashboard without losing the current research view.

---

# 21. REQUIRED ALLOCATION DEFENSE ANALYSIS

For every company, the allocation defense page must contain the following sections.

## 21.1 Allocation summary

Display:

| Metric                | Value               |
| --------------------- | ------------------- |
| Suggested allocation  | X%                  |
| Company score         | X/100               |
| Sector weight         | X%                  |
| Maximum company limit | X%                  |
| Risk classification   | Low / Medium / High |
| Valuation assessment  | Defined methodology |
| Research confidence   | High / Medium / Low |

Do not fabricate any score or metric.

The page must explain how each displayed value was calculated.

## 21.2 Why this percentage?

Generate a detailed, company-specific explanation addressing:

1. Why the company qualifies for its current allocation.

2. Which positive factors support the weight.

3. Which risks limit the weight.

4. How valuation affects the weight.

5. How sector exposure affects the weight.

6. How the company compares with other companies in the same sector.

7. Why the model did not assign a higher percentage.

8. Why the model did not assign a lower percentage.

9. What new evidence could justify an increase or decrease.

10. Whether the allocation is constrained by a portfolio limit.

The explanation must be specific to the company's actual financial profile and portfolio context.

Avoid generic statements such as:

* "The company has strong fundamentals, so it gets 8%."

* "The company has good growth, so it is a top pick."

* "The company has a good valuation, so it deserves a higher allocation."

Replace generic explanations with evidence-backed reasoning.

## 21.3 Allocation contribution breakdown

Display the factors contributing to the allocation.

Example structure:

| Factor               | Score / assessment | Impact on allocation          | Explanation |
| -------------------- | ------------------ | ----------------------------- | ----------- |
| Business quality     | Verified score     | Positive / Neutral / Negative | Evidence    |
| Earnings growth      | Verified score     | Positive / Neutral / Negative | Evidence    |
| Valuation            | Assessment         | Positive / Neutral / Negative | Evidence    |
| Financial strength   | Assessment         | Positive / Neutral / Negative | Evidence    |
| Risk                 | Assessment         | Positive / Neutral / Negative | Evidence    |
| Sector concentration | Assessment         | Positive / Neutral / Negative | Evidence    |
| Research confidence  | Assessment         | Positive / Neutral / Negative | Evidence    |

Do not use arbitrary numerical impact values unless the model explicitly calculates them.

If the impact is qualitative, explain the qualitative methodology.

## 21.4 Allocation calculation trace

Provide an auditable breakdown of the allocation.

Display:

1. Initial company score.

2. Relevant factor scores.

3. Risk adjustments, if any.

4. Valuation adjustments, if any.

5. Diversification adjustments, if any.

6. Sector and company constraints.

7. Final normalized allocation.

Example:

```
Base model score: 78
Valuation adjustment: -5
Risk adjustment: -3
Diversification adjustment: -2
Adjusted model score: 68

Final normalized allocation: 7.5%
```

The above values are illustrative only.

The actual dashboard must calculate these values using a documented and consistent formula.

If the allocation is constrained by a maximum limit, explicitly display:

"Calculated unconstrained weight: X%"
"Applied maximum company limit: Y%"
"Final allocation: Z%"

If the allocation is not constrained, state that.

Do not imply that a factor adjustment was calculated when it was only a qualitative judgment.

---

# 22. DEFEND AGAINST ALTERNATIVE ALLOCATIONS

The allocation defense page must answer the following counterfactual questions.

## 22.1 Why not allocate more?

Title:

**Why Not Increase Allocation?**

Analyze:

* Valuation risk.

* Earnings uncertainty.

* Financial leverage.

* Cyclicality.

* Sector concentration.

* Business concentration.

* Liquidity considerations, where relevant.

* Governance or disclosure concerns.

* Portfolio concentration constraints.

* Lack of sufficient research evidence.

Explain the actual factors relevant to the company.

Do not assume that every company should have a higher allocation.

## 22.2 Why not allocate less?

Title:

**Why Not Reduce Allocation?**

Analyze:

* Business quality.

* Financial strength.

* Earnings visibility.

* Growth potential.

* Valuation support.

* Diversification benefits.

* Relative positioning within the sector.

* Available evidence supporting the company's inclusion.

Do not force a positive justification when the evidence does not support a meaningful allocation.

## 22.3 Why not assign 0%?

Title:

**Why Is the Company Included Instead of Being Placed on the Watchlist?**

Explain:

* Eligibility criteria met.

* Financial evidence supporting inclusion.

* Research confidence.

* Risks that remain unresolved.

* Conditions under which the company would move to the watchlist.

If the company receives 0%, replace this section with:

**Why Does the Model Assign 0%?**

Explain the evidence-based reasons for exclusion, insufficient confidence, or constraint-driven allocation.

---

# 23. COMPARATIVE DEFENSE

Compare the selected company with relevant companies in the same sector.

Include:

| Metric                    | Selected company | Peer 1 | Peer 2 | Peer 3 |
| ------------------------- | ---------------- | ------ | ------ | ------ |
| Revenue growth            | Value            | Value  | Value  | Value  |
| EBITDA margin             | Value            | Value  | Value  | Value  |
| ROCE / appropriate metric | Value            | Value  | Value  | Value  |
| Valuation multiple        | Value            | Value  | Value  | Value  |
| Debt / risk metric        | Value            | Value  | Value  | Value  |
| Suggested allocation      | Value            | Value  | Value  | Value  |

Use only comparable metrics.

For financial institutions and specialized sectors, use relevant industry-specific measures.

Explain:

* Relative strengths.

* Relative weaknesses.

* Differences in valuation.

* Differences in earnings visibility.

* Why the selected company receives its relative weight.

Do not use a peer comparison to create an automatic winner ranking.

Avoid unsupported claims that one company is definitively better.

---

# 24. ALLOCATION SENSITIVITY ANALYSIS

Include an interactive sensitivity section.

Allow the user to view how the suggested allocation could change under documented alternative assumptions.

Example scenarios:

### Scenario 1: Base case

Use the default strategy and assumptions.

### Scenario 2: Valuation-sensitive

Apply a stronger penalty or constraint to companies with elevated valuation risk, using a defined methodology.

### Scenario 3: Growth-priority

Increase the model's relative emphasis on credible earnings growth while retaining risk and concentration controls.

### Scenario 4: Risk-controlled

Increase the relative emphasis on financial strength and reduce concentration limits, using documented assumptions.

For every scenario:

* Show the allocation.

* Explain the assumptions.

* Display the changed factors.

* Show the resulting sector weight.

* Explain which risks are increased or reduced.

Do not claim the scenarios predict actual future returns.

## Sensitivity table

Display:

| Scenario            | Suggested allocation | Difference vs base | Primary reason        |
| ------------------- | -------------------- | ------------------ | --------------------- |
| Base                | X%                   | —                  | Default methodology   |
| Valuation-sensitive | X%                   | +/- X%             | Valuation assumptions |
| Growth-priority     | X%                   | +/- X%             | Growth assumptions    |
| Risk-controlled     | X%                   | +/- X%             | Risk constraints      |

All figures must be generated from actual model calculations or clearly marked as illustrative.

---

# 25. EVIDENCE-BASED DEFENSE

Every important argument on the allocation defense page must be connected to supporting evidence.

For each key claim, provide:

* Source title.

* Source organization.

* Publication date.

* URL.

* Relevant financial year or quarter.

* Whether the information is historical, current, guidance, or an estimate.

* Evidence confidence, where appropriate.

### Evidence classification

Use these labels:

* Verified company disclosure.

* Audited financial information.

* Regulatory disclosure.

* Independent analyst estimate.

* Management guidance.

* Analytical calculation.

* Market commentary.

* Unverified public claim.

Do not treat an analyst target price as verified future performance.

Do not use a source merely because it supports the desired allocation.

Include material evidence that challenges the allocation where it is relevant.

## 25.1 Defense conclusion

At the bottom of the page, generate:

**Allocation Defense Summary**

Include:

* Assigned percentage.

* Two to five strongest supporting factors.

* Two to five major limiting factors.

* Most important valuation assumption.

* Most important risk assumption.

* What could justify increasing the weight.

* What could justify reducing the weight.

* Research confidence.

* Final limitations.

Use a neutral analytical tone.

Do not use language such as:

* "This stock will definitely perform."

* "This is the best company."

* "You should invest this exact percentage."

* "The stock is guaranteed to deliver returns."

Use evidence-based wording such as:

* "The model assigns this weight because..."

* "The allocation is constrained by..."

* "A higher allocation would require..."

* "The weight could be reassessed if..."

---

# 26. HTML INTERACTIVE IMPLEMENTATION

Implement the allocation defense functionality in the HTML.

## 26.1 Main portfolio table

Add a new column:

**Allocation Defense**

Each row must contain:

```
<button
  class="defend-allocation-btn"
  data-company-id="unique-company-id">
  Defend Allocation %
</button>
```

Use a stable, unique company ID.

Do not use unsafe HTML string interpolation for untrusted company names.

## 26.2 Dedicated defense view

When the button is clicked:

1. Identify the selected company.

2. Load the company's allocation defense data.

3. Display the dedicated defense page or full-screen panel.

4. Display the company's allocation percentage.

5. Display the methodology and supporting evidence.

6. Display the comparison and sensitivity analysis.

7. Provide a Back button.

8. Ensure the selected company is clearly identified.

9. Preserve the portfolio dashboard filters where technically feasible.

10. Do not display information belonging to another company.

## 26.3 Defense view navigation

Include:

* Back to Dashboard.

* Company navigation: Previous / Next, if implemented.

* Jump to Allocation Summary.

* Jump to Calculation Trace.

* Jump to Comparative Defense.

* Jump to Risk Analysis.

* Jump to Evidence.

* Print Defense Report.

Use accessible navigation and keyboard-friendly controls.

## 26.4 Dedicated page URL (optional)

If implementing separate pages or routes, use a safe company identifier.

Example:

```
company-defense.html?company=company-a
```

The page must validate the requested company ID and display only matching data.

If a single standalone HTML file is required, implement the defense page as an in-page view or hash-based navigation.

Do not claim that a separate HTML file exists unless it is actually generated.

## 26.5 Defense report export

Provide an option to:

* Print the selected company's allocation defense.

* Export the selected company's defense data to CSV, where feasible.

* Copy the allocation defense summary.

* Save or download the HTML document if the environment supports file generation.

The report must clearly identify the research date and model assumptions.

---

# 27. PORTFOLIO STRATEGY CONTROL PANEL

Add a dedicated panel titled:

**Portfolio Strategy & Allocation Rules**

Display:

* Strategy name.

* Investment horizon.

* Risk preference.

* Maximum company allocation.

* Maximum sector allocation.

* Allocation scoring criteria.

* Valuation treatment.

* Financial risk treatment.

* Diversification rules.

* Eligibility criteria.

* Watchlist rules.

Provide an **"Explain Strategy"** button.

When clicked, open a strategy explanation page or expandable section that explains:

* How the allocation is calculated.

* Why the model uses the selected criteria.

* How the strategy can fail.

* Which assumptions are most influential.

* What the model does not evaluate.

* Which inputs the user can change.

The strategy explanation must be separate from individual company defense pages.

---

# 28. FINAL QUALITY CHECK FOR ALLOCATION DEFENSE

Before finalizing the HTML, validate the following:

### Allocation consistency

* Every allocated company has a working "Defend Allocation %" button.

* Every defense page displays the correct company.

* Every defense page displays the correct suggested allocation.

* The sum of company allocations reconciles to the modeled allocation universe.

* Sector weights reconcile with company weights.

* Constraints are correctly applied.

* The displayed calculation trace matches the actual methodology.

### Research consistency

* Each major allocation reason is supported by evidence or clearly labeled analytical judgment.

* No invented financial metrics.

* No invented URLs.

* No unsupported broker claims.

* No misleading comparisons.

* No false certainty in forward estimates.

* Material negative evidence is not omitted.

### Usability

* Buttons work.

* Back navigation works.

* Company search and filters remain functional.

* The page is responsive.

* Missing data is clearly identified.

* Source links are accessible.

* Print layout is readable.

* The user can distinguish research facts from analytical conclusions.

# FINAL INSTRUCTION

Create an interactive portfolio allocation dashboard that does more than display percentages.

For every company, the dashboard must answer:

**"Why does this company receive this percentage, what limits its allocation, what evidence supports the decision, and what would need to change for the percentage to be revised?"**

The allocation defense feature must be an integral part of the HTML output, not a generic afterthought.

Generate a transparent, auditable, interactive, and professionally designed research dashboard with a clearly defined portfolio strategy and an evidence-based allocation defense page for each company.

## Recommended user experience

The final HTML should work like this:

## Company Allocation Dashboard

Interactive workflow preview

Demo

#### Company A

IT Services • Example

## 8.0%

Fundamental score

78/100

Risk level

Moderate

Defend Allocation %

Illustrative UI only. The actual generated HTML should open the corresponding company defense view.

#### Allocation Defense

Company A

# Why 8.0%?

Allocation Defense & Portfolio Weight Justification

#### 1. Why this percentage?

Explain the company-specific factors supporting the weight, valuation considerations, risk constraints, and diversification effect using verified data.

#### 2. Why not 12%?

Explain the limiting factors, such as concentration, valuation sensitivity, or uncertainty, based on the documented methodology.

#### 3. Why not 4%?

Explain the evidence supporting inclusion and the contribution to the model portfolio.

#### 4. Calculation trace

Base score

78

Adjustments

Defined by model

Final allocation

8.0%

#### 5. Evidence & Sources

Annual reports, financial statements, investor presentations, broker research, and dated calculations.

View Example Defense Report

### Three important additions for your use case

1. Allocation strategy should be adjustable: You should be able to change the maximum allocation per company from 10% to 5%, 8%, or another value and compare the resulting model weights.

2. Defense must compare alternatives: The page should explain why a stock receives 8% rather than 5% or 12%, not just repeat the same investment thesis.

3. Defense should be evidence-based: If a broker report, financial forecast, or management commentary supports the rationale, the report should link to the actual source and identify the date.

Suggested enhancement: Add a "Challenge This Allocation" button alongside "Defend Allocation %." It can open a structured counterargument page that looks specifically for evidence against the proposed weight, such as valuation risk, declining cash flow, margin pressure, or sector concentration. This creates a more balanced research process rather than relying only on the reasons supporting the original allocation.
