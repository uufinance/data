# Economic Data (with APIs)

!!! tip
    FRED requires an API key — register at <a href="https://fred.stlouisfed.org/docs/api/api_key.html" target="_blank">fred.stlouisfed.org/docs/api/api_key.html</a>. The other sources below (ECB, Bundesbank, IMF, OECD, BIS) provide open API access without authentication.

### Quick Comparison

| Source | Coverage | API Format | Auth Required |
|--------|----------|------------|---------------|
| FRED | 800,000+ US & intl series | REST JSON | API key |
| IMF | 190+ countries (WEO, IFS, DOTS) | REST JSON | No |
| OECD | OECD members + partners | SDMX | No |
| BIS | Global banking, credit, FX | SDMX | No |
| ECB | Euro area monetary/financial | SDMX | No |
| Eurostat | EU member states & candidates | JSON/SDMX | No |
| Bundesbank | Germany & Europe | REST | No |

---

- <a href="https://fred.stlouisfed.org/" target="_blank">FRED (Federal Reserve Economic Data)</a> <span class="badge badge-api">API</span> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> — 800,000+ U.S. and international time series from 100+ sources (Fed, BLS, BEA, Census, etc.). Updated daily. Includes <a href="https://alfred.stlouisfed.org/" target="_blank">ALFRED</a> (Archival FRED) for point-in-time vintage data, letting you see what data was available on any historical date (useful for avoiding look-ahead bias). <a href="https://fred.stlouisfed.org/docs/api/fred/" target="_blank">API</a> with Python access via <a href="https://pypi.org/project/fredapi/" target="_blank">`fredapi`</a>, which supports both current data and ALFRED revisions. Covers interest rates, inflation, employment, GDP, money supply, and more.
- <a href="https://research.stlouisfed.org/econ/mccracken/fred-databases/" target="_blank">FRED-MD / FRED-QD</a> <span class="badge badge-csv">CSV</span> <span class="badge badge-us">US</span> — Pre-assembled "big data" macro panels drawn from FRED, designed for macroeconomic factor modeling and forecasting research. **FRED-MD**: 128 monthly U.S. macro series from 1959-present, updated monthly with real-time vintages. **FRED-QD**: 248 quarterly series from 1959:Q1, organized into 14 groups (NIPA, industrial production, employment, interest rates, prices, exchange rates, stock markets, and more). Both are directly downloadable as CSV. By McCracken & Ng (2016, *Journal of Business & Economic Statistics*; 2020, NBER WP 26872).
- <a href="https://data.imf.org/" target="_blank">IMF Data</a> <span class="badge badge-api">API</span> <span class="badge badge-global">Global</span> — International Monetary Fund datasets including the World Economic Outlook (WEO), International Financial Statistics (IFS), Direction of Trade Statistics (DOTS), and Balance of Payments (BOP). Covers macroeconomic indicators, trade flows, exchange rates, and financial soundness for 190+ countries. <a href="https://datahelp.imf.org/knowledgebase/articles/667681-using-json-restful-web-service" target="_blank">API</a> (JSON RESTful).
- <a href="https://data-explorer.oecd.org/" target="_blank">OECD Data Explorer</a> <span class="badge badge-api">API</span> <span class="badge badge-global">Global</span> — Economic, social, and environmental statistics for OECD member and partner countries. Covers GDP, trade, employment, education, health, environment, and more. <a href="https://data-explorer.oecd.org/developers/" target="_blank">API</a> (SDMX).
- <a href="https://data.bis.org/" target="_blank">BIS Statistics</a> <span class="badge badge-api">API</span> <span class="badge badge-global">Global</span> — International banking, derivatives, debt securities, credit, property prices, and exchange rate data from the Bank for International Settlements. Covers cross-border financial flows and global liquidity. <a href="https://data.bis.org/topics" target="_blank">API</a> (SDMX).
- <a href="https://data.ecb.europa.eu/" target="_blank">ECB Statistical Data Warehouse</a> <span class="badge badge-api">API</span> — Euro area monetary, financial, and economic statistics from the European Central Bank. Updated daily. Covers exchange rates, interest rates, monetary aggregates, balance of payments, and banking data. API access (SDMX).
- <a href="https://ec.europa.eu/eurostat/web/main/data/database" target="_blank">Eurostat</a> <span class="badge badge-api">API</span> <span class="badge badge-global">Global</span> — Official statistical office of the European Union, providing data on EU member states and candidate countries. Covers national accounts, employment, prices, trade, population, regional statistics, and more. Free API access in JSON and SDMX formats; Python access via <a href="https://pypi.org/project/eurostat/" target="_blank">`eurostat`</a>.
- <a href="https://www.bundesbank.de/en/statistics/time-series-databases" target="_blank">Deutsche Bundesbank Time Series</a> <span class="badge badge-api">API</span> — German and European economic and financial statistics. Covers capital markets, banking, money markets, public finances, and external sector data. API access.
- <a href="https://cepr.org/voxeu/columns/euro-area-monetary-policy-event-study-database" target="_blank">Euro Area Monetary Policy Event-Study Database (EA-MPD)</a> — High-frequency intraday data on the impact of ECB monetary policy announcements on euro area and global financial markets, covering both conventional and unconventional policy. Data is <a href="https://www.ecb.europa.eu/pub/pdf/annex/Dataset_EA-MPD.xlsx" target="_blank">downloadable as Excel</a> from the ECB website; the VoxEU column provides further explanation of the dataset construction and coverage. By Altavilla et al.
- <a href="https://sites.google.com/site/istrefiklodiana/ea-ced" target="_blank">Euro Area Communication Event-Study Database (EA-CED)</a> — High-frequency data on financial market movements around 304 ECB Governing Council meetings and ~5,100 inter-meeting communication events (speeches, interviews) by ECB Governing Council members. Covers 47 euro area financial variables from January 1999 to February 2024. By Istrefi, Odendahl & Sestieri (Banque de France Working Paper No. 859; CEPR DP No. 19242).
- <a href="https://www.ecb.europa.eu/stats/policy_and_exchange_rates/euro_reference_exchange_rates/html/index.en.html" target="_blank">Euro Foreign Exchange Reference Rates</a> — Daily reference exchange rates for currencies vis-à-vis the euro, published by the ECB.

## Python Examples

```python
# FRED — fetch 10-Year Treasury rate
from fredapi import Fred
fred = Fred(api_key="your_key")
df = fred.get_series("GS10")
```

```python
# IMF — fetch IFS data (e.g., US Consumer Price Index)
import requests
url = "http://dataservices.imf.org/REST/SDMX_JSON.svc/CompactData/IFS/Q.US.PCPI_IX"
data = requests.get(url).json()
```

---
**See also**: [Macroeconomic & Country-Level Data](macro-country-data.md) for country-level indicators, distances, and historical macro datasets.
