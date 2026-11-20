# European Football Transfer Market Analysis (Excel)

**Business question:** Is Europe a net importer or exporter of football talent, which countries drive the spending, and how did the market change between the 2021/22 and 2022/23 seasons?

**Stack:** Excel · data cleaning and lookups · pivot-style aggregation · charts
**Data:** 3,349 country-to-country transfer routes with number of transfers and total club-to-club compensation, for two seasons

---

## Key findings

| KPI | 2021/22 | 2022/23 |
|---|---|---|
| Transfers **into** European countries | 10,744 | 11,148 |
| Transfers **out of** European countries | 9,034 | 9,358 |
| **Net player balance** | **+1,710 (net importer)** | **+1,790 (net importer)** |
| Total spending on incoming transfers | 5.70 bn | 6.18 bn (+8 %) |
| Net transfer balance (spend − income) | +169 M | +89 M |

1. **Europe is a consistent net importer** of players, and both volume and spending grew in 2022/23.
2. **England's spending almost doubled:** 1.15 bn → **2.17 bn** on incoming transfers, with a net spend of **1.53 bn** in 2022/23. That is more than the whole European market's net spend.
3. **The top-5 market changed.** Spain spent the most per player in 2021/22 (2.5 M average). In 2022/23 Spain moved to **net seller** (−210 M), while England led on both volume (1,020 players) and average fee (2.1 M).
4. **Selling leagues fund buying leagues.** Portugal (−526 M net in 2022/23), the Netherlands (−275 M) and Belgium act as talent exporters to the big five.

## Data quality and cleaning

- Filled in missing continent values by looking them up from the `Countries` reference table.
- Reviewed the data for missing values and errors before aggregating.
- **Caveat:** every transfer count in the raw data is an even number, which suggests that each transfer may be counted twice (once from each side). Absolute counts should be checked against the source before they are reported. Ratios and rankings are not affected.

## Files

| File | Content |
|---|---|
| [`data.xlsx`](data.xlsx) | Raw dataset (transfer routes + country reference table) |
| [`Transfer_Analysis_Summary.xlsx`](Transfer_Analysis_Summary.xlsx) | Cleaned data, Europe-level balance, country table, top-5 charts for both seasons |

*Dataset: 365 Data Science, used as a guided case study. Amounts are shown in the dataset's currency units.*
