# Company Information

Resources for identifying companies, accessing regulatory filings and financial statements, retrieving annual reports, and linking firm-level data across databases.

| Topic | Description |
|-------|-------------|
| [Company Filings (SEC EDGAR)](filings.md) | SEC financial statements, filings, insider transactions, fund holdings |
| [Annual Reports](../annual-reports.md) | PDF annual reports for large global companies |
| [Identifiers & Data Linking](../identifiers.md) | CIK, GVKEY, CUSIP, ISIN — how to link datasets across sources |

## Industry Classification

### Hoberg & Phillips — Text-Based Network Industry Classifications (TNIC)

<a href="https://hobergphillips.tuck.dartmouth.edu/" target="_blank">Hoberg & Phillips</a> <span class="badge badge-csv">CSV</span> <span class="badge badge-us">US</span> — Text-Based Network Industry Classifications (TNIC) and product market similarity scores derived from 10-K product description text. Covers U.S. public firms. Widely used as an alternative to SIC and NAICS codes for measuring industry competition, product differentiation, and peer firm identification. (<a href="https://hobergphillips.tuck.dartmouth.edu/industrydat.htm" target="_blank">Data download</a>)

The TNIC approach classifies firms into industries based on the similarity of their product descriptions in annual 10-K filings, rather than using fixed codes assigned by regulatory agencies. This allows industries to evolve over time as firm product portfolios change, and captures competitive relationships that SIC/NAICS codes miss.

A new Embeddings-based TNIC (ETNIC) is available in a preliminary release. (<a href="https://hobergphillips.tuck.dartmouth.edu/tnic_doc2vec.html" target="_blank">Data download</a>)

**Key references**:

- Hoberg, G. and Phillips, G. (2010). Product Market Synergies and Competition in Mergers and Acquisitions: A Text-Based Analysis. *Review of Financial Studies*, 23(10), 3773–3811.
- Hoberg, G. and Phillips, G. (2016). Text-Based Network Industries and Endogenous Product Differentiation. *Journal of Political Economy*, 124(5), 1423–1465.
- Hoberg, G. and Phillips, G. (2024). Scope, Scale and Competition: The 21st Century Firm. *Journal of Finance*, 80(1), 415-466.

---
**See also**: [Data Collections](../researcher-data.md) for general-purpose data repositories | [WRDS](../../wrds/index.md) for Compustat and other company-level databases.
