# Commodities & Futures Data

## CFTC Commitment of Traders (COT) Reports <span class="badge badge-api">API</span> <span class="badge badge-csv">CSV</span> <span class="badge badge-python">Python</span> <span class="badge badge-us">US</span>

The <a href="https://www.cftc.gov/MarketReports/CommitmentsofTraders/index.htm" target="_blank">Commitments of Traders (COT)</a> reports are published weekly by the U.S. Commodity Futures Trading Commission (CFTC). They provide a breakdown of open interest positions in U.S. futures and options markets, classified by trader type. The data reflects positions as of each Tuesday and is released every Friday at 3:30 PM Eastern time. COT data is widely used in finance research to study hedging activity, speculative positioning, commodity market sentiment, and the role of different trader categories in price formation.

The CFTC publishes four types of COT reports, each offering a different level of trader disaggregation and market coverage:

### Legacy Report

The oldest and broadest COT report, available since **January 1986**. It classifies reportable traders into two categories: **Commercial** (hedgers — producers, merchants, processors, and users of the physical commodity) and **Non-Commercial** (speculators — typically managed money and other financial traders). The Legacy report covers both physical delivery contracts (agricultural, energy, metals) and non-physical financial contracts (currencies, interest rates, equity indices), making it the most comprehensive in terms of market coverage. Available in short and long format, futures-only and futures-and-options combined.

### Disaggregated Report

Published since **September 2009** (with data back to June 2006), this report provides greater transparency by splitting traders into four categories: **Producer/Merchant/Processor/User**, **Swap Dealers**, **Managed Money**, and **Other Reportables**. This allows researchers to distinguish between, for example, commodity index swap dealers and traditional commercial hedgers — a distinction that is not possible in the Legacy report. The Disaggregated report covers **physical delivery commodity contracts only** (agriculture, energy, metals, softs). Available in short and long format.

### Traders in Financial Futures (TFF) Report

The TFF report covers **financial (non-physical) futures contracts only** — currencies, interest rates, equity indices, and other financial instruments. It classifies traders into four categories: **Dealer/Intermediary** (sell-side institutions), **Asset Manager/Institutional** (pension funds, insurance companies, mutual funds), **Leveraged Funds** (hedge funds, CTAs, CPOs), and **Other Reportables**. Available since **June 2006** in long format only. Particularly useful for research on institutional positioning in interest rate and equity index futures.

### Supplemental (Commodity Index Trader) Report

Introduced in **January 2007** in response to the growth of commodity index investing, this report adds a **Commodity Index Trader (CIT)** category to the Legacy classifications for **13 select agricultural commodity markets**. It allows researchers to separate index fund positions from traditional commercial and speculative positions — useful for studying the financialization of commodity markets. Available in short format only, futures-and-options combined.

### Report Comparison

| Report | Market Coverage | Trader Categories | Data Since | Format |
|--------|----------------|-------------------|------------|--------|
| **Legacy** | Physical + financial contracts | Commercial, Non-Commercial | Jan 1986 | Short & Long |
| **Disaggregated** | Physical commodity contracts only | Producer/Merchant, Swap Dealer, Managed Money, Other | Jun 2006 | Short & Long |
| **TFF** | Financial contracts only | Dealer, Asset Manager, Leveraged Fund, Other | Jun 2006 | Long only |
| **Supplemental (CIT)** | 13 agricultural commodities | Commercial, Non-Commercial, Index Trader | Jan 2007 | Short only |

## Accessing COT Data

### CFTC Website & Bulk Downloads

- <a href="https://www.cftc.gov/MarketReports/CommitmentsofTraders/index.htm" target="_blank">COT Reports Main Page</a> — Current and historical COT reports in all four formats. Includes links to bulk CSV downloads for each report type, with data going back to 1986 (Legacy) or 2006 (Disaggregated, TFF, Supplemental).
- <a href="https://www.cftc.gov/MarketReports/CommitmentsofTraders/HistoricalViewable/index.htm" target="_blank">Historical Viewable Reports</a> — Weekly COT reports in HTML format, viewable directly in the browser. Each report covers a single reporting week, with all historical reports available as compressed annual files.
- <a href="https://www.cftc.gov/data" target="_blank">Data at CFTC</a> — Overview page for all CFTC data products, including COT reports, swaps data, and market surveillance information.

### CFTC Public Reporting API

The CFTC provides free programmatic access to all COT report data through a <a href="https://publicreporting.cftc.gov/stories/s/Commitments-of-Traders/r4w3-av2u/" target="_blank">Socrata-based (SODA) API</a> at `publicreporting.cftc.gov`. The API supports filtering, sorting, and pagination via standard query parameters, making it straightforward to retrieve data for specific contracts, date ranges, or trader categories.

!!! tip
    The CFTC API requires no authentication or API key — you can start querying immediately.

- <a href="https://publicreporting.cftc.gov/stories/s/Commitments-of-Traders/r4w3-av2u/" target="_blank">COT API Landing Page</a> — Entry point for all COT datasets with links to individual report APIs (Legacy, Disaggregated, TFF, Supplemental) in both futures-only and combined variants.
- <a href="https://publicreporting.cftc.gov/stories/s/User-s-Guide/p2fg-u73y/" target="_blank">User's Guide</a> — Documentation on how to use the CFTC public reporting platform, including API query syntax, filtering options, and export formats.
- <a href="https://dev.socrata.com/foundry/publicreporting.cftc.gov/6dca-aqww" target="_blank">Legacy Futures-Only API Docs</a> — Socrata developer documentation for the Legacy Futures-Only endpoint, with example queries and field descriptions.

### Python Access

- <a href="https://github.com/NDelventhal/cot_reports" target="_blank">`cot_reports`</a> — Open-source Python library for fetching all CFTC COT report types directly into pandas DataFrames. Supports Legacy (futures-only and combined), Disaggregated (futures-only and combined), TFF (futures-only and combined), and Supplemental reports. (<a href="https://pypi.org/project/cot-reports/" target="_blank">PyPI</a>)

```bash
pip install cot_reports
```

## Additional Resources

- <a href="https://www.cmegroup.com/tools-information/quikstrike/commitment-of-traders.html" target="_blank">CME Group QuikStrike COT Tool</a> — Interactive visualization of CFTC COT data for CME-listed contracts, with configurable charts and historical comparisons.
- <a href="https://www.financialresearch.gov/hedge-fund-monitor/datasets/tff/" target="_blank">Office of Financial Research (OFR) — TFF Data</a> — The OFR (U.S. Treasury) provides downloadable Traders in Financial Futures datasets with visualization tools, useful for research on hedge fund and institutional positioning.
- <a href="https://cot-reports.com/" target="_blank">COT-Reports.com</a> — Free COT analysis platform with 10 years of historical data, charts, tables, and analysis tools covering 340+ futures markets.

## ESMA Commitment of Traders Reports <span class="badge badge-csv">CSV</span> <span class="badge badge-global">Global</span>

The <a href="https://registers.esma.europa.eu/publication/searchRegister?core=esma_registers_coder58" target="_blank">ESMA Commitment of Traders Reports</a> are the European equivalent of the CFTC COT reports, published weekly by the European Securities and Markets Authority (ESMA) under MiFID II Article 58. Trading venues in the EU are required to submit weekly reports on aggregate open positions held by different categories of market participants in commodity derivatives and emission allowances. ESMA centrally publishes these reports, covering European commodity futures markets that are largely absent from CFTC data.

The reports classify position holders into five categories:

- **Investment firms or credit institutions**
- **Investment funds** (including UCITS and AIFs)
- **Other financial institutions**
- **Commercial undertakings** (producers, processors, and commercial end-users)
- **Operators with compliance obligations** under the EU Emissions Trading Scheme (ETS)

Data reflects positions as of the close of business each Friday. Compared to CFTC reports, the ESMA data uniquely identifies EU ETS compliance operators as a separate trader category, and covers European energy, agricultural, and carbon derivatives markets.

## European Electricity Market Data

### ENTSO-E Transparency Platform <span class="badge badge-api">API</span> <span class="badge badge-csv">CSV</span> <span class="badge badge-global">Global</span>

The <a href="https://transparency.entsoe.eu/" target="_blank">ENTSO-E Transparency Platform</a> provides free access to European electricity market data, published by the European Network of Transmission System Operators for Electricity. Covers actual and forecast electricity generation, cross-border flows, day-ahead prices, load, and balancing data for 35+ European countries. Data is published with a delay of 24 hours or less. Free registration required for API access.

- <a href="https://transparency.entsoe.eu/dashboard/show" target="_blank">Transparency Platform Dashboard</a> — Interactive dashboard with real-time and historical electricity data. Data downloadable as CSV directly from the web interface.
- <a href="https://transparency.entsoe.eu/content/static_content/Static%20content/web%20api/Guide.html" target="_blank">ENTSO-E RESTful API</a> — Programmatic access to all transparency data via a RESTful API. Requires a free account and API security token. Python access via the <a href="https://pypi.org/project/entsoe-py/" target="_blank">`entsoe-py`</a> client library.

```bash
pip install entsoe-py
```

---
**See also**: [Asset Classes](assets/index.md) for an overview of all asset class data | [Economic & Macroeconomic Data](economic/index.md) for macro drivers of commodity markets | [Python Tools & Books](python-tools.md) for general financial data packages.
