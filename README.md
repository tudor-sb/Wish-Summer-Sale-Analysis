# Wish Marketplace — Summer Catalog & Ad Boosts Efficiency Analysis

An Excel-based commercial analysis of 1,341 summer apparel listings on the Wish marketplace (representing a minimum of 6.46M units sold and 52.36M € in estimated gross revenue). The project evaluates how revenue is distributed across price and customer rating tiers, and tests whether paid promotions (`Ad Boosts`) and reference discounts drive measurable revenue gains.

## Repository Contents

* `Wish_Catalog_Analysis.xlsx` — Complete Excel workbook containing the executive dashboard, pivot tables, unit revenue comparisons, cleaned dataset, and statistical checks.

## Workbook Structure

1. **Summary** — Executive KPI cards, performance breakdown by price and rating segments, two comparative charts (`Ad Boost Upside vs Downside` and `Product Performance and Ad Boosts Usage`), and a 3-point Action Matrix.
2. **Pivots** — Interactive pivot tables with slicers analyzing high-volume sales rates (`>= 1,000` units sold) across rating tiers, reference discounts, and `Ad Boost` status.
3. **Economics** — Segment-level comparisons between promoted and unpromoted listings, measuring average gross revenue per product and `Ad Effect / Product`.
4. **Products** — Cleaned dataset with standardized currency formatting, estimated gross revenue (`Price × Units Sold`), and engineered tier columns for price, rating, and sales volume.
5. **Appendix** — Quartile distributions and outlier checks used to validate segment averages.

## Key Findings

* **Productivity vs. Total Volume:** `Average` price items (`5–10 €`) generate the largest share of total revenue (**55%**, or **28.99M €**), while `Premium` items (`> 10 €`) deliver the highest average revenue per listing at **46,725 €** — **3.7x** higher than `Cheap` products (**12,513 €**) and above `Average` products (**40,715 €**, or **3.3x** `Cheap`).
* **Misallocated Ad Spend on Cheap & Low-Rated Items:** Sellers promote `Cheap` products most heavily (**60%** use `Ad Boosts`, vs. **42%** for `Average` and **40%** for `Premium`), yet promoted `Cheap` listings generate **6,547 € less** per product on average than unpromoted ones. `Low Rating` (`< 3.5`) products show a similar negative differential (**-9,103 €** per product).
* **Where Ad Boosts Align with Positive Performance:** Across standalone tiers, only `Premium` (**+5,605 €** per product) and `Average Rating` (`3.5–3.99`, **+2,936 €** per product) show a positive average `Ad Effect / Product`. Cross-segment pivot analysis confirms that positive bulk-sales lift (**+7% to +9%**) is concentrated in `Average` and `Premium` price items (`> 5 €`) paired with `Average Ratings`.
* **Selection Bias on High-Rated Listings:** `High Rating` (`4.0–5.0`) products show a negative differential when promoted (**-6,840 €** per product). Because well-rated listings tend to sell organically, `Ad Boosts` appear to be activated reactively on items that are stagnating. *(35 unrated listings generated only 8,135 € in total gross revenue and were excluded from the rating segmentation.)*
* **Reference Discount Effectiveness:** `Average Rating` products drive **52%** of total revenue (**27.26M €**), and **81%** of their high-volume sales occur without inflated reference discounts. Discounts correlate with higher bulk-sales rates only when paired with a `High Rating`.

## Actionable Recommendations

1. **Ad Boost Allocation:** Cut back `Ad Boosts` on `Cheap` and `Low Rating` products and reallocate ad spend toward `Average–Premium` products (`> 5 €`) with `Average Ratings` (`3.5–3.99`), where promoted listings outperform unpromoted ones.
2. **Pricing & Discount Strategy:** Phase out artificial reference discounts on `Low` and `Average Rating` products to protect price credibility, reserving price promotions for `High Rating` listings.
3. **Product Selection:** Enforce a minimum `3.5` rating gate (after an initial 10–20 reviews so new listings are not locked out) before enabling `Ad Boosts`, and scale `High Rating` (`>= 4.0`) products primarily through organic visibility.

## Methodology & Limitations

* **Observational Data (Correlation vs. Causation):** The dataset is a static marketplace snapshot rather than a randomized A/B test. Differences between promoted and unpromoted listings reflect observed patterns—including potential selection bias—and should be validated via controlled testing before scaling.
* **Gross Revenue Scope:** Product costs, platform commissions, and ad spend are not available in the dataset; all financial metrics represent estimated gross revenue (`Price × Units Sold`) rather than net profit.
* **Lower-Bound Volume Estimates:** Wish reports units sold in rounded brackets (e.g., `100`, `1,000`, `5,000+`), making total volume and gross revenue figures conservative baseline estimates.