# Bonds & Fixed Income

Free and open-access data sources for fixed income markets, including yield curves, credit spreads, corporate bond factors, and return predictors.

!!! tip
    For licensed fixed income databases, see [Mergent FISD](../wrds/databases/mergent-fisd.md), [TRACE](../wrds/databases/trace.md), and [Bond Returns](../wrds/databases/bond-returns.md) on WRDS.

## Yields & Spreads

- <a href="https://fred.stlouisfed.org/categories/115" target="_blank">U.S. Treasury Yield Curves (FRED)</a> <span class="badge badge-api">API</span> <span class="badge badge-csv">CSV</span> <span class="badge badge-us">US</span> <span class="badge badge-bonds">Bonds</span> — Daily constant-maturity Treasury yields (1-month to 30-year) from the Federal Reserve's H.15 release. Coverage: 1962–present (varies by maturity). Key series: DGS1, DGS2, DGS5, DGS10, DGS30. Free via the FRED website, API, or the <a href="https://pypi.org/project/fredapi/" target="_blank">`fredapi`</a> Python package. Widely used for term structure research, risk-free rate estimation, and yield curve modeling.
- <a href="https://fred.stlouisfed.org/series/BAMLC0A0CM" target="_blank">ICE BofA Corporate Bond Indices (FRED)</a> <span class="badge badge-api">API</span> <span class="badge badge-csv">CSV</span> <span class="badge badge-us">US</span> <span class="badge badge-bonds">Bonds</span> — Option-adjusted spreads (OAS) for investment-grade (BAMLC0A0CM) and high-yield (BAMLH0A0HYM2) corporate bonds, published by ICE/BofA and available free via FRED. Daily, 1996–present. Standard measures for credit risk research, default risk pricing, and business cycle analysis. Also includes indices by maturity and rating bucket.

## Factor Data & Return Predictors

- <a href="https://openbondassetpricing.com/" target="_blank">Open Source Bond Asset Pricing</a> <span class="badge badge-csv">CSV</span> <span class="badge badge-us">US</span> <span class="badge badge-bonds">Bonds</span> — Replication data and code for corporate bond factors, including daily TRACE bond panels, bond-Compustat/CRSP links, and 341 bond/stock predictors. By Dickerson, Mueller & Robotti (2023). (<a href="https://openbondassetpricing.com/code/" target="_blank">Code</a>)

---
**See also**: [Equities & Asset Pricing](asset-pricing.md) for equity factor data | [WRDS Fixed Income databases](../wrds/databases/index.md) for licensed bond data (Mergent FISD, TRACE, Bond Returns).
