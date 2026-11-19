# Deep Research Prompt 2: Independent Verification of Defence and Aerospace Company News

## Role

Act as a forensic corporate research analyst and financial fact-checker.

I will provide a company-wise news report discovered from X, LinkedIn, company websites and other sources during the last one month.
Please access the news report from URL: https://sites.google.com/view/indiandefenceindustryintellige/full-page-embed and verify the authenticity of the news by cross-checking with multiple credible sources, including official company press releases, regulatory filings, and reputable financial news outlets.
Your job is to independently verify the claims, identify errors and repetitions, establish the strongest available evidence, and distinguish confirmed business developments from unverified claims.

Do not simply summarise or accept the previous report. Challenge it.

## Research scope

Use the exact date range and company list in the supplied report. Verify every material claim, prioritising claims about:
- Contract awards and order values.
- Government approvals and procurement decisions.
- Export orders.
- Customer relationships and programme participation.
- Product testing, qualification and commercial production.
- Capacity expansion and capex.
- Quarterly financial performance and guidance.
- Order-book additions, cancellations and execution delays.
- Negative news and material risks.

## Verification hierarchy

Use the following evidence hierarchy:

**Grade A — Primary documentary evidence**
- NSE/BSE corporate filings.
- Official company press releases and investor disclosures.
- Government or Ministry of Defence announcements.
- Official customer or procurement-agency announcements.
- Publicly available contract documents or formal award announcements.

**Grade B — Credible independent corroboration**
- Reputable business publications and established news organisations.
- Official OEM, supplier or business-partner announcements that independently corroborate the development.

**Grade C — Attributable but not independently confirmed**
- Specific statements by company management, executives or authorised representatives.
- Social-media posts that make identifiable factual claims but lack documentary corroboration.

**Grade D — Unverified**
- Anonymous claims, speculative posts, unsupported financial estimates and promotional content.

A claim should not be classified as a confirmed fact merely because an official account or multiple social-media accounts repeated it. Seek the underlying evidence.

## Mandatory checks for every material claim

1. Find the original announcement.
2. Confirm the publication date and whether it falls within the research period.
3. Verify the exact listed entity involved.
4. Confirm the customer, project, product or government agency.
5. Validate the announced contract value, quantities, delivery timeline and company-attributable share.
6. Determine whether the development is a firm order, purchase order, tender, MoU, letter of intent, trial, approval or potential opportunity.
7. Check whether the information was already disclosed before the research period.
8. Search for later updates, corrections, cancellations or contradictory disclosures.
9. Check whether multiple sources are merely reproducing the same original announcement.
10. Record any unresolved ambiguity.

For consortiums, subsidiaries, joint ventures and group companies, establish which legal entity actually receives the order or revenue.

## Financial and commercial verification

Where a report claims a business or financial impact:

- Check the latest available financial results, investor presentation and exchange filings.
- Compare the announced order with the company's existing order book where reliable data is available.
- Distinguish contract value, order-book addition, annual revenue, lifetime programme value and total consortium value.
- Do not assume the entire order value will be recognised as revenue in the next financial year.
- Do not assume margins are known when they have not been disclosed.
- Treat derived calculations as estimates and show the formula and assumptions.
- Use INR crore consistently when appropriate.
- Do not convert foreign currency using an unstated or arbitrary exchange rate.

## Required output

### A. Verification table

| Company | Original Claim | Original Date | Best Evidence | Evidence Grade | Verification Result | Corrected Facts | Remaining Uncertainty |

Use these verification results:
- Confirmed.
- Partially confirmed.
- Not independently verified.
- Incorrect or misleading.
- Previously known; not a new development.
- Duplicate report.
- Superseded or cancelled.
- Unable to verify due to source-access limitations.

Provide direct URLs to the primary source and the best independent corroborating source, wherever available.

### B. Material corrections
List all important errors, inflated order values, incorrect company attributions, misleading headlines, wrong dates and unsupported assumptions found in the initial report.

Explain the correction and cite the supporting evidence.

### C. Confirmed news shortlist
Produce a clean list of the most important developments supported by Grade A evidence or strong Grade B corroboration.

For each item, include:
- Company and date.
- Exact confirmed facts and figures.
- Customer or programme.
- Nature of the development.
- Contract value and attributable share, if established.
- Delivery period, if disclosed.
- Why the development matters.
- Source links.

### D. Unresolved claims
List material claims that remain unverified. Explain what evidence is missing and whether the claim should be excluded from further business analysis.

### E. Negative and contradictory evidence
Identify cancellations, delays, execution problems, negative disclosures, corrections and other facts that weaken or contradict a positive narrative.

### F. Final clean research dataset
Produce a deduplicated, company-wise table containing only correctly attributed developments, with a separate field for evidence status.

Preserve unverified claims in a separate section rather than silently deleting them.

### G. Company coverage audit
Verify that every unique company from the original watchlist was assessed. Distinguish companies with no confirmed developments from companies for which the available evidence was insufficient.

## Rules

- Research independently; do not trust the initial report by default.
- Never upgrade an unverified claim to a fact merely because it sounds plausible.
- Do not invent citations or imply that a source confirms more than it actually says.
- Cite every material factual conclusion.
- Use the latest available correction or update where applicable.
- Do not make share-price predictions or buy/sell recommendations.

## Final objective

Deliver an evidence-clean dataset that can be used as the factual foundation for a third-stage business and investment-impact assessment. Accuracy and correct attribution matter more than the number of positive news items.