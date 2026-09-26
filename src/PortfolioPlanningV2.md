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
