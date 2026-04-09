# Perplexity Pitch Contest — BlackRock Long Position

**Nicholas Hawkins | Hawkins Holdings | April 2026**

---

## Investment Thesis

> *BlackRock (NYSE: BLK) is the highest-quality capital allocation in the asset management sector for 2026 — a fee-compounding platform at the intersection of indexed investing, private markets, and financial operating-system infrastructure.*

Currently trading ~21% below its 52-week high, BLK offers a technically attractive entry point with **+23.7% consensus upside** to the analyst average price target of $1,239.26 (19 analysts, Benzinga, April 8, 2026).

---

## Repository Structure

```
├── models/
│   ├── BLK_DCF_Model_Hawkins_Holdings_2026.xlsx   ← DCF model v1 (6 sheets)
│   └── BLK_DCF_Model_April_2026_v2.xlsx           ← DCF model v2 (final)
├── pitch-materials/
│   ├── blk_flagship_asset_allocation.html          ← Slide deck (existing)
│   ├── blk-intelligence-dashboard/
│   │   └── blk-intelligence-dashboard.html         ← Interactive dashboard (Deliverable 1)
│   └── BlackRock-Initial-Inquiry.pdf               ← Initial research brief
├── docs/
│   ├── BLK_Data_Patch_April8_2026.md              ← Canonical data corrections ← READ FIRST
│   ├── BLK-Investment-Analysis-Guidance.pdf        ← Analysis framework
│   ├── BLK_DCF_Scenario_Assumptions.docx          ← DCF assumptions (v1)
│   ├── BlackRock-BLK-2026-Perplexity-Implementation-Plan.pdf
│   ├── BlackRock-BLK-DCF-Evidence-Ledger.docx
│   └── BlackRock-BLK-Financial-Profile-FY2022-FY2025.docx
├── README.md
└── SOURCES.md
```

---

## DCF Model — Sheet Index

| Sheet | Description |
|---|---|
| **Cover** | Navigation, key metrics snapshot, investment thesis |
| **Income Statement** | FY2022A–FY2027E: Revenue, Adj. EBITDA, Adj. EPS, AUM |
| **FCF Bridge** | NOPAT → FCFF → FCFE with all adjustments |
| **WACC Calculator** | CAPM cost of equity, cost of debt — Bear/Base/Bull |
| **DCF Valuation** | Terminal value (perpetuity), intrinsic value per share |
| **Sensitivity Tables** | WACC × terminal growth rate → IV/share (3-color heatmap) |

---

## Key Financial Data (FY2025 Actuals — April 8, 2026 Canonical)

| Metric | Value | YoY |
|---|---|---|
| **AUM** | **$14.04T** | +21.6% |
| Revenue | $24.22B | +18.7% |
| Adj. Operating Margin | 44.1% | −40bps |
| Adj. EPS | $48.09 | +10.3% |
| Full-Year Net Inflows | $698.3B | Record |
| iShares Net Inflows | $527B | Record |
| Tech/Aladdin Revenue | $2.0B | +24% |
| Aladdin ACV Growth | +31% (incl. Preqin) | — |
| Cash & Equivalents | $11.5B | — |

> **Note:** FY2024 AUM was $11.55T. Any reference to "$11.6T AUM" in earlier drafts is the prior-year figure and should be treated as stale.

---

## Strategic Transaction Timeline

| Transaction | Close | AUM Added | Deal Value | Impact |
|---|---|---|---|---|
| GIP (Global Infrastructure Partners) | Oct 2024 | ~$70B | **~$12.5B** ($3B cash + ~$9.5B stock) | 2nd-largest infrastructure manager globally |
| Preqin | Mar 2025 | Data platform | $3.2B | Private-markets data integrated into Aladdin |
| HPS Investment Partners | Jul 2025 | **$118B private credit AUM** | — | Credit franchise scaled above $220B total |

> **Correction applied:** GIP deal value was previously misquoted as "$3B." The cash component was $3B; total consideration was ~$12.5B including stock. See `docs/BLK_Data_Patch_April8_2026.md`.

---

## Valuation Scenarios (April 8, 2026 Reference Price: $1,001.54)

| Scenario | WACC | Terminal g | Intrinsic Value / Share | Upside / (Downside) |
|---|---|---|---|---|
| Bear | 11.0% | 2.0% | ~$820 | −18.1% |
| Base | 9.5% | 2.5% | ~$1,180 | +17.8% |
| Bull | 8.0% | 3.25% | ~$1,490 | +48.8% |

*See `Sensitivity Tables` sheet for full WACC × g matrix across all scenarios.*

---

## Three-Layer Conviction Stack

1. **AUM Compounding Machine** — iShares #1 ETF globally ($5.5T ETF AUM), $698B record inflows, 3–5% organic growth target; total AUM $14.04T (FY2025)
2. **Strategic Platform Transformation** — GIP (~$12.5B, Oct 2024) + Preqin ($3.2B, Mar 2025) + HPS ($118B private credit, Jul 2025) pivot BLK to alternatives + data; $423.6B alternatives AUM
3. **Aladdin Technology Moat** — Infrastructure layer for $21.6T+ in client assets; Preqin integration unlocks private-markets data monetization; tech revenue $2.0B (+24%), ACV +31% (FY2025)

---

## Analyst Consensus (April 8, 2026 — Canonical)

- **Consensus PT:** $1,239.26 (19 analysts, Benzinga)
- **Rating:** Strong Buy (15 Buys, 2 Holds, 0 Sells, per Ticker Nerd)
- **High PT:** $1,456 (B of A Securities, Oct 15, 2025)
- **Current Price:** $1,001.54 (April 8, 2026)
- **Implied Upside to Avg. PT:** +23.7%

### Most Recent Analyst Actions (April 8, 2026)

| Firm | Action | Target | Date | Change |
|---|---|---|---|---|
| Barclays | Overweight | $1,290 | Apr 8, 2026 | Maintained (↓ from $1,350) |
| Goldman Sachs | Buy | $1,181 | Apr 7, 2026 | Cut (↓ from ~$1,277) |
| Morgan Stanley | Overweight | $1,368 | Apr 1, 2026 | Cut (↓ from $1,550) |
| UBS | Buy | $1,280 | Feb 23, 2026 | Upgrade |
| Keefe, Bruyette & Woods | Outperform | $1,340 | Jan 16, 2026 | Maintained |

> **Note:** The $1,239.26 consensus already incorporates the Goldman and Morgan Stanley cuts. The previous README cited $1,325.90 / 38.5% upside — those figures were April 3 pre-cut.

---

## Comparable Companies (Re-Rating Peer Set)

| Company | Ticker | AUM | Fwd P/E | EV/EBITDA | Rev Growth |
|---|---|---|---|---|---|
| **BlackRock** | **BLK** | **$14.04T** | **~22x adj.** | **17.6x** | **+18.7%** |
| Blackstone | BX | ~$1.1T | 29.5x | 19.4x | — |
| KKR | KKR | ~$640B | 39.0x | — | — |
| Apollo | APO | ~$785B | 19.9x | — | — |
| T. Rowe Price | TROW | ~$1.6T | 9.7x | — | — |

*T. Rowe Price at 9.7x = valuation floor for pure-play traditional managers without platform transition. BX/KKR at 29–39x = re-rating ceiling as BLK alternatives + tech mix is credited by the market.*

---

## Sources

See [SOURCES.md](SOURCES.md) for full citation index.

Primary sources:
- [BlackRock Q4 2025 Earnings Release (Jan 15, 2026)](https://www.blackrock.com/corporate/newsroom/press-releases/article/corporate-one/press-releases/blackrock-reports-fourth-quarter-2025)
- [BLK 10-K FY2025 (SEC EDGAR via StockTitan)](https://www.stocktitan.net/sec-filings/BLK/10-k-black-rock-inc-files-annual-report-d280a370171b.html)
- [Benzinga BLK Analyst Ratings (Apr 8, 2026)](https://www.benzinga.com/quote/BLK/analyst-ratings)
- [Ticker Nerd BLK Forecast](https://tickernerd.com/stock/blk-forecast/)
- [GuruFocus WACC & Forward P/E](https://www.gurufocus.com/term/wacc/BLK)
- [AlphaSpread Relative Valuation](https://www.alphaspread.com/security/nyse/blk/relative-valuation)
- [StockAnalysis.com — BLK Forecast](https://stockanalysis.com/stocks/blk/forecast/)

---

## Disclaimer

*This repository is prepared for the Perplexity Pitch Contest (April 2026) and does not constitute investment advice. All projections are based on publicly available data and analyst consensus estimates.*

---

*Built with Perplexity — demonstrating AI-augmented institutional-grade investment analysis.*  
*Last updated: April 8, 2026*
