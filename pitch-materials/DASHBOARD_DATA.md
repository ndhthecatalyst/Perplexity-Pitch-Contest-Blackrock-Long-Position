# BLK Intelligence Dashboard — Data Reference

**Canonical data for `blk-intelligence-dashboard.html`**  
**Reference date: April 8, 2026**  
All figures in this file are post-patch and ready to wire directly into the dashboard.

---

## PITCH_STATE Object (JavaScript)

```js
const PITCH_STATE = {
  // Market Snapshot
  ticker:           'BLK',
  exchange:         'NYSE',
  company:          'BlackRock, Inc.',
  price:            1001.54,
  dayHigh:          1017.15,
  dayLow:           995.78,
  marketCap:        164900000000,        // ~$164.9B
  consensusTarget:  1239.26,
  consensusUpside:  0.2373,              // +23.7%
  analystCount:     19,
  referenceDate:    'April 8, 2026',
  earningsDate:     new Date('2026-04-21T08:00:00'), // Q1 2026 estimate

  // AUM & Financial
  aumTotal:         14.04,               // $T FY2025
  aumETF:           5.5,                 // $T (US $3.9T + Intl $1.6T)
  aumAlternatives:  0.4236,             // $T ($423.6B)
  aladdinAUM:       21.6,               // $T managed on Aladdin platform

  // Navigation
  activeTab:        'overview'
};
```

---

## MODULE A — Market Snapshot Hero

| Field | Value | Style |
|---|---|---|
| Ticker | BLK · NYSE | `--text-xs`, muted, uppercase tracked |
| Company | BlackRock, Inc. | Instrument Serif, `--text-xl` |
| Last price | **$1,001.54** | JetBrains Mono, `--text-2xl`, gold |
| Day range | $995.78 – $1,017.15 | `--text-sm`, muted |
| Market cap | ~$164.9B | `--text-base` |
| Consensus target | **$1,239.26** | gold badge |
| Implied upside | **+23.7%** | success-colored pill |
| Reference date | April 8, 2026 | `--text-xs`, faint |
| Earnings status | PRE-Q1 2026 EARNINGS | warning badge |
| Analyst count | 19 analysts | `--text-xs`, muted |

---

## MODULE B — Investment Thesis Panel

### Card 1 — Structural Market Dominance

- **Title:** Structural Market Dominance
- **Body:** iShares anchors $5.5T in ETF AUM — 3 of every 10 ETF dollars globally flow through BlackRock infrastructure. The passive shift is structural, not cyclical, and iShares' 12% organic asset growth in 2025 proves the engine accelerates even in uncertainty.
- **Data badge:** `$14.04T AUM` ← (corrected from $11.6T)
- **Sparkline data (7 points, 2019–2025):**
  ```js
  [7.43, 8.68, 10.01, 8.59, 10.01, 11.55, 14.04]
  // Labels: ['2019','2020','2021','2022','2023','2024','2025']
  ```
  Note: The 2022 dip (8.59) should remain visible — it strengthens the narrative.

### Card 2 — The Illiquidity Premium Capture

- **Title:** The Illiquidity Premium Capture
- **Body:** GIP (~$12.5B acquisition, Oct 2024), Preqin ($3.2B, Mar 2025), and HPS ($118B private credit AUM, Jul 2025) create a private credit + infrastructure + data trifecta that no passive-only incumbent can replicate.
- **Data badge:** `$423.6B Alternatives AUM` (or "$400B+ private AUM target" per management)
- **Acquisition timeline (4 nodes, horizontal CSS):**

  | Node | Label | Date | Detail |
  |---|---|---|---|
  | 1 | GIP | Oct 2024 | ~$12.5B; 2nd-largest infra mgr globally |
  | 2 | Preqin | Mar 2025 | $3.2B; private-markets data into Aladdin |
  | 3 | HPS | Jul 2025 | $118B private credit AUM; credit platform >$220B |
  | 4 | FY2025 | Dec 2025 | $423.6B alternatives AUM; $698B record inflows |

### Card 3 — The Operating System Play

- **Title:** The Operating System Play
- **Body:** Aladdin manages $21.6T of client assets across 200+ institutions. The Preqin data layer turns the platform into a two-sided marketplace. SaaS-like recurring revenue — $2.0B in FY2025, up 24%, ACV +31% including Preqin — shields against AUM-fee compression.
- **Data badge:** `$21.6T Aladdin AUM`
- **Revenue mix donut (Chart.js doughnut, 3 segments):**

  ```js
  data:   [76, 8, 16],
  labels: ['Investment Advisory Fees', 'Technology (Aladdin/Preqin)', 'Distribution & Other'],
  colors: ['#d19900', '#4f98a3', '#524f48']
  // Values represent approximate % of FY2025 revenue ($24.22B)
  // Tech segment: $2.0B / $24.22B ≈ 8%
  ```

---

## MODULE C — Valuation Panel

### Sub-module C1 — Scenario Matrix

| Scenario | Badge color | Target | Upside | Key Assumption |
|---|---|---|---|---|
| Bear | `--color-error` | ~$820 | −18.1% | 20% AUM compression (market correction), HPS/GIP integration 6-month delay, multiple de-rates to 17x P/E |
| Base | `--color-primary` (gold) | ~$1,180 | +17.8% | Management guidance execution: 5–7% organic fee growth, 16% Aladdin ACV, 44–45% margins |
| Bull | `--color-success` | ~$1,490 | +48.8% | Aladdin ACV sustains 20%+ via Preqin, alternatives AUM → $850B, multiple re-rates toward BX/KKR |

Footnote: "Targets are internal proprietary estimates derived from a 5-year DCF + Comparable Company Analysis. Not a solicitation. As of April 8, 2026."

### Sub-module C2 — Valuation Bridge Chart (Horizontal Bar)

```js
// Chart.js horizontal bar
labels: ['Current Price', 'Peer Median P/E', 'DCF Intrinsic (Base)', 'Bull Case Target'],
data:   [1001.54, 1050, 1180, 1490],   // peer median estimated at ~1050
colors: ['#8a877e', '#4f98a3', '#d19900', '#6daa45']
// Note: Peer median reflects BLK at 22x fwd P/E vs. comparable blended peer
```

### Sub-module C3 — Comparable Company Table

```
Sortable. Sticky header. Rows expand on click (inline drawer).
```

| Company | Ticker | AUM | Fwd P/E | EV/EBITDA | Rev Growth | Analyst Target |
|---|---|---|---|---|---|---|
| **BlackRock** | **BLK** | **$14.04T** | **~22x** | **17.6x** | **+18.7%** | **$1,239** |
| Blackstone | BX | ~$1.1T | 29.5x | 19.4x | — | — |
| KKR | KKR | ~$640B | 39.0x | — | — | — |
| Apollo | APO | ~$785B | 19.9x | — | — | — |
| T. Rowe Price | TROW | ~$1.6T | 9.7x | — | — | — |

**Drawer text per row (progressive disclosure):**

- **Blackstone (BX):** Largest alternative asset manager by market cap at $137B. 29.5x P/E reflects full credit for its pure-play alternatives franchise. BLK's growing alternatives AUM ($423.6B) is the primary catalyst for re-rating toward this range.
- **KKR:** 39x P/E premium reflects insurance balance sheet integration (Global Atlantic) and private wealth channel growth. Serves as the bull-case multiple ceiling for BLK's combined Aladdin + alternatives re-rating.
- **Apollo (APO):** 19.9x P/E reflects a credit-heavy mix with AUM-correlated fee revenue. Closest structural analog to BLK's HPS private credit build-out ($118B private credit AUM at close).
- **T. Rowe Price (TROW):** 9.7x P/E illustrates the valuation floor for pure-play traditional active managers with no platform transition. BLK currently trades well above this, justified by its technology and alternatives mix.

---

## MODULE D — Analyst Intelligence Panel

### Left: Dot-Plot Data (SVG / Chart.js Scatter)

```js
// Price targets as of April 8, 2026
// Solid = last 30 days; Faint = older
const analystTargets = [
  // Last 30 days (solid dots)
  { target: 1290, firm: 'Barclays',        date: '2026-04-08', recency: 'recent' },
  { target: 1181, firm: 'Goldman Sachs',   date: '2026-04-07', recency: 'recent' },
  { target: 1368, firm: 'Morgan Stanley',  date: '2026-04-01', recency: 'recent' },

  // Older (faint dots)
  { target: 1280, firm: 'UBS',             date: '2026-02-23', recency: 'old' },
  { target: 1340, firm: 'KBW',             date: '2026-01-16', recency: 'old' },
  { target: 1209, firm: 'TD Cowen',        date: '2026-01-14', recency: 'old' },
  { target: 1350, firm: 'Barclays',        date: '2026-01-08', recency: 'old' }, // prior action
  { target: 1456, firm: 'B of A',          date: '2025-10-15', recency: 'old' },
  { target: 1486, firm: 'Morgan Stanley',  date: '2025-10-15', recency: 'old' }, // prior target
  { target: 1300, firm: 'Consensus',       date: '2026-04-08', recency: 'consensus' },
];

// X-axis range: $900 – $1,550
// Current price vertical line: $1,001.54 (gold)
// Consensus marker: $1,239.26 (dashed teal)
```

### Right: Recent Analyst Actions (5 rows)

| Firm | Action | Target | Date |
|---|---|---|---|
| Barclays | Overweight | $1,290 | Apr 8, 2026 |
| Goldman Sachs | Buy | $1,181 | Apr 7, 2026 |
| Morgan Stanley | Overweight | $1,368 | Apr 1, 2026 |
| UBS | Buy | $1,280 | Feb 23, 2026 |
| KBW | Outperform | $1,340 | Jan 16, 2026 |

Pill badge logic:
- Overweight / Outperform / Buy → `--color-success` pill
- Neutral / Hold → `--color-text-muted` pill
- Underweight / Sell → `--color-error` pill

---

## MODULE E — Catalyst Countdown

### Card E1

- **Header:** Next Catalyst: Q1 2026 Earnings
- **Target date:** `new Date('2026-04-21T08:00:00')`
- **Status badge:** `PRE-EARNINGS · LONG THESIS ACTIVE` (warning color)
- **Display:** DD : HH : MM : SS — counting down in real time via `setInterval`

### Card E2 — Earnings Watch List

1. AUM net flows: above/below $50B quarterly threshold
2. Aladdin revenue run-rate and client ACV additions — target 16%+ organic
3. GIP/HPS/Preqin integration update: synergy timeline, cost disclosure
4. Fee rate trajectory: basis-point compression vs. mix shift to higher-fee private markets
5. Management guidance on 2026 margin: hold 44–45%+ adj. operating margin
6. Commentary on regulatory environment (EU, U.S. asset manager oversight, FSOC)

---

## MODULE F — Risk Register

| # | Risk | Severity | Mitigant |
|---|---|---|---|
| 1 | Fee rate compression from passive shift | Medium | Private markets mix shift, Aladdin SaaS recurring revenue |
| 2 | AUM outflows in risk-off environment | High | Multi-asset, global client diversification; $698B proven inflow engine |
| 3 | M&A integration execution (GIP, HPS, Preqin) | High | 20-year acquisition track record; early HPS synergy data positive |
| 4 | Regulatory / ESG political pressure | Medium | Geographic and product diversification; FSOC engagement history |
| 5 | Key-person risk (Fink succession) | Medium | Deep bench (Kapito, Martin); institutionalized processes |
| 6 | Tech platform competition (Aladdin moat erosion) | Medium | Network effects, switching costs, Preqin data integration |
| 7 | Rate environment / duration risk on bond AUM | Medium | Fee revenue not mark-to-market sensitive; tech/alts hedge |
| 8 | Valuation premium vs. peers | Low | Justified by Aladdin SaaS re-rating potential; ~22x vs. 9.7x floor |

---

## MODULE G — Perplexity Process Timeline

| Stage | Icon | Title | Description | Output Badge |
|---|---|---|---|---|
| 1 | Search | Deep Research Initiation | Multi-round web search establishing BLK's competitive position, AUM data, Aladdin architecture, and M&A timeline using Perplexity Search | Evidence Spine · 40+ Sources |
| 2 | Database | Premium Data Pull | Structured financial data extraction: quarterly financials, segment revenue, analyst estimates, institutional holders, and price history via Perplexity's Premium Data tools | Financial Dataset · Apr 8 Mark |
| 3 | Chart | Financial Modeling | DCF model construction, comparable company analysis, and sum-of-parts valuation with Perplexity Computer executing Python calculations and scenario analysis | 3-Scenario Valuation Model |
| 4 | Document | IC Memo Drafting | Investment Committee memo written with AI-assisted synthesis of all research strands, structured per industry convention with bull/base/bear framing | Institutional IC Memo |
| 5 | Monitor | Live Intelligence Dashboard | This interactive artifact — price tracking, analyst intelligence, catalyst monitoring, and risk register — built with Perplexity Computer | You Are Here |

### "What Perplexity Made Possible" tiles:

1. "Compressed 40+ hours of research into a single iterative session"
2. "Real-time data synchronization from April 2 initial inquiry to April 8 refresh"
3. "Financial modeling and artifact generation in a unified workflow"

---

## Design Tokens Reminder

```css
/* Dark mode (default) */
--color-bg:             #0f0e0c;
--color-surface:        #161513;
--color-surface-2:      #1d1c19;
--color-surface-offset: #232118;
--color-text:           #e8e5df;
--color-text-muted:     #8a877e;
--color-text-faint:     #524f48;
--color-primary:        #d19900;   /* Gold */
--color-primary-hover:  #b07a00;
--color-secondary:      #4f98a3;   /* Teal */
--color-success:        #6daa45;
--color-error:          #dd6974;
--color-border:         rgba(232, 229, 223, 0.10);  /* oklch fallback */

/* Light mode overrides */
--color-bg:             #f4f2ee;
--color-surface:        #f9f8f5;
--color-primary:        #b07a00;
--color-text:           #1a1914;
```

---

## Font Loading (Both CDNs)

```html
<!-- Fontshare (Satoshi — body) -->
<link rel="preconnect" href="https://api.fontshare.com">
<link href="https://api.fontshare.com/v2/css?f[]=satoshi@400,500,700&display=swap" rel="stylesheet">

<!-- Google Fonts (Instrument Serif — display; JetBrains Mono — data) -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Instrument+Serif&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
```

---

*This file is the single source of truth for all data wired into `blk-intelligence-dashboard.html`.*  
*Last updated: April 8, 2026*
