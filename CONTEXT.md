# Reno Source Financial Projections V4.0 — Context

## What Changed from V3 to V4

### Key Updates
1. **Two Months of Actuals**: Now includes M1 (April 2026) and M2 (May 2026) actual operating results
2. **Revised Forward Projections**: M3–M24 projections updated based on observed performance trends
3. **P&L Structure**: Table now shows `M1 Proj | M2 Proj | M1 Actual | M2 Actual | M3 ... M24`
4. **New Charts**: Added revenue and EBITDA bar charts with actuals highlighted in orange
5. **Updated Unit Economics**: Reflects actual M1/M2 data points
6. **Slider Behavior**: Sliders only affect M3-M24 (forward projections); actuals and historical projections stay fixed

### M1 & M2 Actuals Summary

**M1 (April 2026)**
- Total Sales: $89,473
- Net Revenue: $71,003
- Gross Margin: 48.4%
- EBITDA: -$110,117
- Marketing Spend: $48,750
- Blended CPC: $0.70

**M2 (May 2026)**
- Total Sales: $372,834
- Net Revenue: $307,201 (4.3× M1)
- Gross Margin: 50.2%
- EBITDA: -$79,547
- Marketing Spend: $112,077
- Blended CPC: $0.86

### Year 1 & Year 2 Totals

**Year 1 (M1–M12) Projected Net Revenue**: $14.0M  
**Year 2 (M13–M24) Projected Net Revenue**: $66.5M

### Model Assumptions

- **Gross Margin**: 45–50% Y1 / 45% Y2
- **AOV Range**: $1,420 (M1 actual) → $1,750 (M24 projected)
- **Blended CPC**: $0.70 (M1 actual) → $1.80 (M24 projected)
- **Breakeven**: Month 6
- **Core Conversion Rate**: 0.06% (M1) → 0.36% (M24)
- **Core CAC**: $1,134 (M1) → $500 (M24)

### Slider Mechanics

The V4 model includes three interactive sliders:

1. **AOV Multiplier** (±20%): Scales average order value for M3-M24 only
2. **Gross Margin Multiplier** (±5%): Adjusts gross margin % for M3-M24 only
3. **CPC Sensitivity** (±25%): Scales the CPC curve and marketing spend for M3-M24 only

**Important**: M1 and M2 actuals are NEVER affected by sliders. M1 Proj and M2 Proj are also fixed (historical projections from v3 model).

### Data Integrity

- All RAW arrays contain exactly 24 values (indices 0-23 = M1-M24)
- `nonMktgOpex` is computed as: `payroll + rent + ccVar + other`
- `EBITDA` = `grossMargin - nonMktgOpex - marketing`
- `Net Income` = `EBITDA - capex`
- Actuals are unaudited and subject to small reconciliation errors

### Files

- `index.html` — Self-contained interactive dashboard (39KB)
- `CONTEXT.md` — This file
- `README.md` — User-facing documentation

### Version History

- **V1.0**: Initial pre-launch model (never released)
- **V2.0**: Launch model (Feb 2026)
- **V3.0**: M1 actuals integrated (April 2026)
- **V3.1**: Minor corrections to M1 data
- **V4.0**: M1 + M2 actuals integrated, full 24-month reforecast (June 2026)

---

**Model Date**: June 6, 2026  
**Prepared By**: Jon Volz (Reno Source)  
**Status**: Confidential — Accredited Investors Only
