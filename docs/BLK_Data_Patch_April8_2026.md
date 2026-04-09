# BLK Data Patch — April 8, 2026 Canonical Corrections

**Author:** Nicholas Hawkins | Hawkins Holdings  
**Date:** April 8, 2026  
**Purpose:** Cross-document data alignment. This document supersedes any conflicting figures in earlier drafts and establishes the canonical data spine for the BLK Intelligence Dashboard and all pitch materials.

---

## Patch 1 — GIP Acquisition Deal Value (HIGH PRIORITY)

**Error in earlier drafts:** "GIP ($3B deal)"  
**Correction:** The GIP acquisition total was **$12.5 billion** ($3.0B in cash + approximately 12 million BLK shares valued at ~$9.5B at close, October 2024). The $3B figure was the cash component only.

| Field | Incorrect | Correct | Source |
|---|---|---|---|
| GIP deal value | $3B | ~$12.5B total ($3B cash + ~$9.5B stock) | [ION Analytics, Jan 2024](https://ionanalytics.com/insights/infralogic/blackrock-to-acquire-gip-for-over-usd-12-5bn/); [Investopedia](https://www.investopedia.com/blackrock-makes-infrastructure-push-with-usd12-5-billion-purchase-of-gip-8425625); [Wind Power Monthly](https://www.windpowermonthly.com/article/1890644/blackrock-closes-12-billion-plus-deal-buy-global-infrastructure-partners) |
| GIP deal close | — | October 2024 | BLK 10-K FY2025 |
| AUM added via GIP | — | ~$70B AUM at close | BLK 10-K FY2025 |
| Deal multiple | — | ~25–29x FY2024E P/FRE | ION Analytics |

**Dashboard impact:** Module B Card 2 body copy and acquisition timeline node.  
**Corrected phrasing for Module B Card 2:** "GIP (~$12.5B acquisition, Oct 2024), Preqin ($3.2B, Mar 2025), HPS ($118B private credit AUM, Jul 2025) create a private credit + infrastructure + data trifecta."

---

## Patch 2 — AUM Badge in Module B Card 1 (HIGH PRIORITY)

**Error in earlier drafts:** "$11.6T AUM (as of latest report)"  
**Correction:** $14.04T as of December 31, 2025 (FY2025 closing AUM). The $11.6T figure approximated FY2024 year-end AUM ($11.55T) and should not appear in any April 2026 materials.

| Field | Incorrect | Correct | Source |
|---|---|---|---|
| Total AUM (latest) | $11.6T | **$14.04T** | [BLK Q4 2025 Earnings Release, Jan 15, 2026](https://www.blackrock.com/corporate/newsroom/press-releases/article/corporate-one/press-releases/blackrock-reports-fourth-quarter-2025) |
| AUM YoY growth | — | +21.6% | Q4 2025 Earnings |
| FY2024 AUM (prior year) | — | $11.55T | BLK Q4 2024 Earnings |

**Dashboard impact:** Module B Card 1 data badge. Module A hero strip references $14.04T as AUM context.

**AUM Context (for Module B Card 1 body copy):**
- Total AUM: **$14.04T** (FY2025)
- iShares ETF AUM: US $3.9T + International $1.6T = **$5.5T**
- Full-year 2025 iShares net inflows: **$527B** (record)
- Organic ETF asset growth: **12%**
- "3 of every 10 ETF dollars globally" remains valid — iShares holds #1 global ETF market share

---

## Patch 3 — Module D Analyst Intelligence Table (HIGH PRIORITY)

**Error in earlier drafts:** Table listed only Barclays (Apr 8). Goldman Sachs and Morgan Stanley actions from the same week were omitted.  
**Source for this patch:** [Benzinga BLK Analyst Ratings, Apr 8, 2026](https://www.benzinga.com/quote/BLK/analyst-ratings); [MarketBeat Morgan Stanley note, Apr 1, 2026](https://www.marketbeat.com/instant-alerts/morgan-stanley-cuts-blackrock-nyseblk-price-target-to-136800-2026-04-01/)

### Corrected Module D Analyst Action Table (5 most recent as of Apr 8, 2026):

| Firm | Action | Target | Date | Change |
|---|---|---|---|---|
| Barclays | Overweight | $1,290 | Apr 8, 2026 | Maintained (↓ from $1,350) |
| Goldman Sachs | Buy | $1,181 | Apr 7, 2026 | Cut (↓ from ~$1,277) |
| Morgan Stanley | Overweight | $1,368 | Apr 1, 2026 | Cut (↓ from $1,550) |
| UBS | Buy | $1,280 | Feb 23, 2026 | Upgrade |
| Keefe, Bruyette & Woods | Outperform | $1,340 | Jan 16, 2026 | Maintained |

**Notes:**
- Goldman Sachs cut to $1,181 is the most bearish current Buy-rated target and the most recent significant cut. It sits notably below the consensus average and will stand out on the dot-plot (correct behavior — illustrates that even the most conservative bull is still +18% above current price).
- Morgan Stanley cut $1,550 → $1,368 on April 1. The $1,550 was Morgan Stanley's prior target (Oct 2025, following Q3 earnings). The new $1,368 still implies ~37% upside from current price.
- **Consensus $1,239.26 from 19 analysts (Apr 8) is CONFIRMED CORRECT** — this figure already incorporates all three of the most recent actions above. Source: [Benzinga](https://www.benzinga.com/quote/BLK/analyst-ratings)

### Dot-Plot Price Range for Module D (Apr 8, 2026):
- Low target: $980 (UBS, Apr 2025 — historical low, show as faint)
- High target: $1,456 (B of A Securities, Oct 2025)
- Consensus: $1,239.26
- Current price: $1,001.54
- Cluster of targets: $1,181 – $1,456 range (most targets in this band)

---

## Patch 4 — Module C Comparable Company Table (MEDIUM PRIORITY)

**Error in earlier drafts:** Used Vanguard, State Street, TROW, and Franklin Templeton as the comp peer set.

**Correction:** Per the BLK Implementation Plan and `BLK_Comps_Table__DCF_Triangulation__April_2026.docx`, the correct peer set for the valuation re-rating narrative is **alternative asset managers + traditional managers**, which frames both the current trough multiple and the bull case re-rating ceiling.

### Corrected Module C Comparable Company Table:

| Company | Ticker | AUM | Fwd P/E | EV/EBITDA | Revenue Growth | Analyst Target |
|---|---|---|---|---|---|---|
| **BlackRock** | **BLK** | **$14.04T** | **~22x adj.** | **17.6x** | **+18.7%** | **$1,239** |
| Blackstone | BX | ~$1.1T | 29.5x | 19.4x | — | — |
| KKR | KKR | ~$640B | 39.0x | — | — | — |
| Apollo | APO | ~$785B | 19.9x | — | — | — |
| T. Rowe Price | TROW | ~$1.6T | 9.7x | — | — | — |

**Rationale:** This peer set makes the re-rating argument explicit and visual. T. Rowe Price at 9.7x shows the valuation floor for pure-play traditional managers with no platform transition. BX at 29.5x and KKR at 39.0x show the ceiling if BLK's alternatives + tech mix is fully credited. BLK at ~22x adj. P/E sits between these poles — which is exactly the investment argument.

**Data sources:**  
- BLK fwd P/E ~22x: [GuruFocus, Apr 2026](https://www.gurufocus.com/term/wacc/BLK)  
- BLK EV/EBITDA 17.6x: [AlphaSpread Relative Valuation, Apr 2026](https://www.alphaspread.com/security/nyse/blk/relative-valuation); [ValueInvesting.io, Apr 2026](https://valueinvesting.io/BLK/valuation/ev_ebitda-multiple)  
- BX 29.5x, KKR 39x, APO 19.9x, TROW 9.7x: Implementation Plan comp table (sourced from AlphaSpread, Apr 2026)

**Dashboard accordion drawer text (per row):**
- **Blackstone (BX):** Largest alternative asset manager by market cap. 29.5x P/E reflects premium for pure-play alternatives franchise. BLK's growing alts mix (currently ~$423B AUM) is the primary re-rating catalyst toward this multiple range.
- **KKR:** 39x P/E premium reflects insurance balance sheet integration and private wealth channel growth. KKR's re-rating serves as the bull-case ceiling for BLK's Aladdin + alternatives mix.
- **Apollo (APO):** 19.9x P/E reflects credit-heavy mix with more AUM-correlated fee revenue. Closest structural analog to BLK's HPS private credit build.
- **T. Rowe Price (TROW):** 9.7x P/E illustrates the valuation floor for pure-play traditional active managers without a platform transition. Serves as the bear-case de-rating anchor.

---

## Patch 5 — HPS AUM Figure (LOW-MEDIUM PRIORITY)

**Conflicting figures across documents:**
- 10-K FY2025 (most authoritative): **$118B private credit AUM** added via HPS Transaction
- Financial profile doc: $165B client AUM (includes committed/unfunded capital)
- Some drafts: $148B

**Resolution:** Use the 10-K figure for financial precision. Use the broader framing for narrative.

| Context | Figure to Use | Rationale |
|---|---|---|
| Acquisition timeline node (Module B, G) | **$118B private credit AUM** | 10-K EDGAR, primary source |
| Narrative context | "BLK's credit franchise scaled above $220B post-HPS" | 10-K: "scaling BLK's credit franchise above $220 billion" |
| Combined private markets | "$423.6B alternatives AUM (FY2025)" | 10-K FY2025, includes GIP + HPS + prior |

---

## Confirmed-Correct Figures (No Changes Required)

The following figures from the original spec are verified against primary sources as of April 8, 2026:

| Field | Value | Source |
|---|---|---|
| Last price (Apr 8) | $1,001.54 | [Benzinga](https://www.benzinga.com/quote/BLK/analyst-ratings) |
| Day range | $995.78 – $1,017.15 | Market data |
| Market cap | ~$164.9B | ~163.4M diluted shares × $1,001.54 |
| Consensus target | $1,239.26 | [Benzinga, Apr 8, 2026](https://www.benzinga.com/quote/BLK/analyst-ratings) |
| Analyst count | 19 | Benzinga |
| Implied upside | +23.7% | ($1,239.26 − $1,001.54) / $1,001.54 |
| FY2025 Revenue | $24.22B | BLK Q4 2025 Earnings |
| FY2025 Adj. EPS | $48.09 | BLK Q4 2025 Earnings |
| Adj. Op. Margin | 44.1% | BLK Q4 2025 Earnings |
| Aladdin AUM managed | $21.6T | BLK disclosures |
| Aladdin ACV growth (FY2025) | +31% incl. Preqin (+16% organic) | BLK 10-K FY2025 |
| Preqin deal value | $3.2B | Press release |
| FY2025 net inflows | $698.3B (record) | BLK Q4 2025 Earnings |
| iShares net inflows (FY2025) | $527B (record) | BLK Q4 2025 Earnings |
| Adj. FCF (FY2025) | $3.55B | BLK 10-K FY2025 |
| Cash & equivalents | $11.5B | BLK Q4 2025 Earnings |
| FY2026E Revenue (consensus) | ~$28.5B | StockAnalysis.com |
| FY2026E Adj. EPS (consensus) | ~$54.44–$54.95 | StockAnalysis / MarketBeat |
| DCF Bear target | ~$820 (−18.1%) | BLK_DCF_Scenario_Assumptions.docx |
| DCF Base target | ~$1,180 (+17.8%) | BLK_DCF_Scenario_Assumptions.docx |
| DCF Bull target | ~$1,490 (+48.8%) | BLK_DCF_Scenario_Assumptions.docx |
| WACC (Bear/Base/Bull) | 11.0% / 9.5% / 8.0% | BLK_DCF_Scenario_Assumptions.docx |
| Terminal growth (Bear/Base/Bull) | 2.0% / 2.5% / 3.25% | BLK_DCF_Scenario_Assumptions.docx |
| Earnings countdown date | ~April 21, 2026 (est.) | Q1 2026 typical window |
| AUM 5-yr CAGR | 10% | BLK 10-K FY2025 |

---

## AUM Sparkline Data — Module B Card 1 (2019–2025)

For the 7-point AUM sparkline (gold line chart, Chart.js):

| Year | AUM ($T) | Source |
|---|---|---|
| 2019 | $7.43 | Annual report |
| 2020 | $8.68 | Annual report |
| 2021 | $10.01 | Annual report |
| 2022 | $8.59 | Annual report (market downturn) |
| 2023 | $10.01 | Annual report |
| 2024 | $11.55 | Annual report |
| 2025 | $14.04 | Q4 2025 Earnings Release |

Note: 2022 dip is accurate and should display — it demonstrates that even in a down market year, BLK maintained net inflows and rebounded strongly. Do not smooth this out.

---

## Revenue Mix Donut — Module B Card 3 (Chart.js Doughnut)

For the 3-segment revenue donut (Aladdin/tech vs. fee revenue vs. other):

| Segment | FY2025 Revenue | % of Total | Color |
|---|---|---|---|
| Investment Advisory & Admin Fees | ~$18.5B | ~76% | Gold (`#d19900`) |
| Technology Services (Aladdin/Preqin) | ~$2.0B | ~8% | Teal (`#4f98a3`) |
| Distribution, Other | ~$3.7B | ~16% | Muted (`#524f48`) |

Source: BLK 10-K FY2025 — "Technology services and subscription revenue reached $2.0 billion, up 24%"  
Note: Technology/Aladdin segment at $2.0B (+24% YoY, ACV +31%) is the highest-growth segment and the re-rating catalyst, even though it is the smallest revenue slice. The visual should convey this dynamic.

---

*Document prepared April 8, 2026. All figures sourced from primary financial disclosures or verified sell-side data aggregators. For the Perplexity Pitch Contest 2026.*
