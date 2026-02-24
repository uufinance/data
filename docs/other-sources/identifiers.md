# Identifiers & Data Linking

When combining data from different sources (e.g., SEC filings with Compustat fundamentals, or Compustat data with analyst forecasts), you need a common identifier to match records. This page provides a quick reference for the most common financial identifiers and how to link datasets.

## Common Identifiers

| Identifier | Assigned by | Scope | Notes |
|------------|-------------|-------|-------|
| **Ticker** | Exchanges | Exchange-specific | Changes over time (mergers, rebranding). Not unique across exchanges. |
| **CIK** | SEC | U.S. SEC filers | Central Index Key. Unique to each filer. Used across all EDGAR data. |
| **GVKEY** | S&P / Compustat | Compustat universe | Permanent company identifier. Does not change with ticker or name changes. |
| **PERMNO** | CRSP | CRSP universe | Permanent security identifier. Unique to each security listing. |
| **CUSIP** | CUSIP Global Services | North America | 9-character identifier for securities. Can be recycled after delisting — not permanent. |
| **ISIN** | National numbering agencies | Global | 12-character international standard (ISO 6166). First 2 characters = country code, next 9 = local identifier (often CUSIP for US), last = check digit. |
| **SEDOL** | London Stock Exchange | UK / international | 7-character identifier widely used in international markets. |
| **LEI** | GLEIF | Global | 20-character Legal Entity Identifier for counterparty identification. |

## Linking Datasets

### SEC EDGAR ↔ Compustat (via CIK)

SEC filings use CIK numbers. To link to Compustat:

1. Use the Compustat **company** table which contains both `gvkey` and `cik`
2. Or use WRDS Audit Analytics tables that include CIK fields — see the [Audit Analytics guide](../wrds/databases/audit-analytics.md) for details

### SEC EDGAR ↔ Tickers

The SEC provides a free CIK-to-ticker mapping:

- <a href="https://www.sec.gov/files/company_tickers.json" target="_blank">company_tickers.json</a> — JSON file mapping CIK numbers to tickers and company names for all SEC filers

### CUSIP ↔ ISIN

For U.S. securities, the ISIN is constructed from the CUSIP:
- ISIN = `"US"` + 9-digit CUSIP + check digit
- Many databases provide both; if you only have one, the conversion is straightforward

## Common Pitfalls

!!! warning
    - **Tickers are not permanent** — companies change tickers (e.g., Facebook → Meta: FB → META). Always use permanent identifiers (GVKEY, PERMNO, CIK) for panel data.
    - **CUSIPs can be recycled** — after a security is delisted, its CUSIP may be reassigned. Use CUSIP + date for unambiguous identification.
    - **One company, multiple securities** — a single company (one GVKEY/CIK) may have multiple stock classes (multiple PERMNOs/CUSIPs). Be explicit about which security you need.
    - **Header vs. body CUSIPs** — some datasets use the 6-character issuer code (header CUSIP), others use the full 9-character security-level CUSIP. Make sure you're matching at the right level.

---
**See also**: [Company Information, Filings & News](company-info-news.md) for SEC EDGAR data and CIK lookups | [WRDS](../wrds/index.md) for Compustat and other database access.
