# Company Filings & Financial Data (SEC EDGAR)

## SEC EDGAR — Company Filings & Financial Data <span class="badge badge-api">API</span> <span class="badge badge-csv">CSV</span> <span class="badge badge-us">US</span>

The <a href="https://www.sec.gov/data-research/sec-markets-data" target="_blank">SEC Data Library</a> provides freely downloadable datasets extracted from filings submitted to the U.S. Securities and Exchange Commission. All data is public and requires no authentication.

!!! tip
    EDGAR APIs are free with no authentication required. Rate limit: 10 requests per second. Include a `User-Agent` header with your name and email in programmatic requests.

- <a href="https://www.sec.gov/edgar/search/" target="_blank">EDGAR Full-Text Search</a> — Search the full text of all SEC electronic filings since 2001, including 10-K, 10-Q, 8-K, proxy statements, and all other SEC forms. Searchable by company, filing type, date range, and keywords.
- <a href="https://www.sec.gov/search-filings/edgar-application-programming-interfaces" target="_blank">EDGAR APIs</a> — Free RESTful JSON APIs for programmatic access to company submissions, financial facts (XBRL), and filing metadata. No authentication or API key required. Includes the Company Facts API, Submissions API, and XBRL Frames API. Max 10 requests/second.
- <a href="https://www.sec.gov/data-research/sec-markets-data/financial-statement-data-sets" target="_blank">Financial Statement Data Sets</a> — Numeric data from the face financials of all public company financial reports filed in XBRL. Covers balance sheets, income statements, and cash flow statements. Updated quarterly.
- <a href="https://www.sec.gov/data-research/sec-markets-data/financial-statement-notes-data-sets" target="_blank">Financial Statement and Notes Data Sets</a> — Detailed text and numeric information from all financial statements and their notes (XBRL). Significantly more comprehensive than the Financial Statement Data Sets. Updated monthly.
- <a href="https://www.sec.gov/data-research/sec-markets-data/financial-statement-data-sets-archive" target="_blank">Financial Statement Data Sets Archive</a> — Archived version of the Financial Statement Data Sets, including numeric and narrative disclosures from all financial statements and their notes.
- <a href="https://www.sec.gov/data-research/sec-markets-data/insider-transactions-data-sets" target="_blank">Insider Transactions Data Sets</a> — Section 16 insider trading filings (Forms 3, 4, and 5) for senior executives, directors, and 10%+ shareholders, covering changes in company stock holdings. Updated quarterly.
- <a href="https://www.sec.gov/data-research/sec-markets-data/edgar-log-file-data-sets" target="_blank">EDGAR Log File Data Sets</a> — Internet search traffic data for EDGAR filings, useful for studying investor attention and information demand. Available from 2003–2017 and 2020–present. Updated quarterly.
- <a href="https://www.sec.gov/data-research/sec-markets-data/number-of-edgar-filings-by-form-type" target="_blank">Number of EDGAR Filings by Form Type</a> — Aggregate counts of EDGAR filings broken down by form type, useful for studying filing trends and regulatory activity.
- <a href="https://www.sec.gov/data-research/sec-markets-data/company-information-about-active-broker-dealers" target="_blank">Company Information About Active Broker-Dealers</a> — Identification and registration data for active SEC-registered broker-dealers.
- <a href="https://www.sec.gov/data-research/sec-markets-data/bankruptcy-cases" target="_blank">Bankruptcy Cases</a> — List of bankruptcy cases for public companies filed under Chapter 11 of the Bankruptcy Code, opened and monitored since fiscal year 2009.
- <a href="https://www.sec.gov/data-research/sec-markets-data/company-information" target="_blank">Company Information (CIK Numbers)</a> — Central Index Key (CIK) numbers, company names, SEC reporting file numbers, and addresses for all SEC-filing companies.

## SEC EDGAR — Capital Formation

- <a href="https://www.sec.gov/data-research/sec-markets-data/form-d-data-sets" target="_blank">Form D Data Sets</a> — Notices of exempt offerings filed under Regulation D (Rule 504, 506(b), 506(c)) and Section 4(a)(5) of the Securities Act. Covers private placements and capital formation. Updated quarterly.
- <a href="https://www.sec.gov/data-research/sec-markets-data/crowdfunding-offerings-data-sets" target="_blank">Crowdfunding Offerings Data Sets</a> — Structured data from Regulation Crowdfunding offering statements, updates, annual reports, and terminations (Form C). Updated quarterly.
- <a href="https://www.sec.gov/data-research/sec-markets-data/regulation-data-sets" target="_blank">Regulation A Data Sets</a> — Data on small securities offerings filed under Regulation A (Forms 1-A, 1-K, 1-Z). Covers Tier 1 and Tier 2 offerings up to $75 million.

## SEC EDGAR — Investment Companies & Funds

- <a href="https://www.sec.gov/data-research/sec-markets-data/form-13f-data-sets" target="_blank">Form 13F Data Sets</a> — Quarterly institutional investor holdings for investment managers with $100M+ in Section 13(f) securities. Covers which institutions hold which stocks. Updated quarterly. See also [Asset Pricing](../asset-pricing.md).
- <a href="https://www.sec.gov/data-research/sec-markets-data/bdc-data-sets" target="_blank">Business Development Company (BDC) Data Sets</a> — Schedule of investments, detailed financial data, and summary non-financial data from BDC XBRL filings.
- <a href="https://www.sec.gov/data-research/sec-markets-data/variable-insurance-product-data-sets" target="_blank">Variable Insurance Product Data Sets</a> — Text and numeric data from variable annuity contract registration forms (Forms N-3, N-4, N-6) filed in XBRL. Updated monthly.
- <a href="https://www.sec.gov/data-research/sec-markets-data/form-n-port-data-sets" target="_blank">Form N-PORT Data Sets</a> — Monthly portfolio holdings data for registered investment companies, covering securities positions, risk metrics, and flow information.
- <a href="https://www.sec.gov/data-research/sec-markets-data/dera-form-n-mfp-data-sets" target="_blank">Form N-MFP Data Sets</a> — Monthly reports from money market funds on portfolio holdings, including fund characteristics and individual security-level data.
- <a href="https://www.sec.gov/data-research/sec-markets-data/form-n-cen-data-sets" target="_blank">Form N-CEN Data Sets</a> — Annual reports from registered investment companies covering fund operations, service providers, and financial information.
- <a href="https://www.sec.gov/data-research/sec-markets-data/mutual-fund-prospectus-risk-return-summary-data-sets" target="_blank">Mutual Fund Prospectus Risk/Return Summary Data Sets</a> — Text and numeric data extracted from the risk/return summary section of mutual fund prospectuses.
- <a href="https://www.sec.gov/data-research/sec-markets-data/money-market-fund-information" target="_blank">Money Market Fund Information</a> — Identification data and aggregate statistics for all money market mutual funds that file Form N-MFP.
- <a href="https://www.sec.gov/search-filings/mutual-funds-search/search-mutual-fund-proxy-voting-records" target="_blank">Form N-PX</a> — Proxy voting records from registered management investment companies and institutional managers on executive compensation matters. Annual filings covering the 12-month period ended June 30. Bulk data can be retrieved via the <a href="https://efts.sec.gov/LATEST/search-index?q=%22N-PX%22&dateRange=custom&startdt=2024-01-01&enddt=2025-01-01&forms=N-PX" target="_blank">EDGAR full-text search API</a>. See <a href="https://doi.org/10.1016/j.jfineco.2024.103810" target="_blank">Shu (2024, <i>Journal of Financial Economics</i>)</a> for an application inferring proxy advisor relationships from N-PX filings to characterize the proxy advice market.
- <a href="https://www.sec.gov/data-research/sec-markets-data/series-and-class-report" target="_blank">Series and Class Report</a> — Identification information for all active registered investment company series and classes that have been issued IDs by the Commission.

## SEC — Market Participants

- <a href="https://www.sec.gov/data-research/sec-markets-data/information-about-registered-investment-advisers-exempt-reporting-advisers" target="_blank">Information About Registered Investment Advisers and Exempt Reporting Advisers</a> — Registration data from Form ADV for investment advisers and exempt reporting advisers, including business operations, assets under management, and disciplinary history.
- <a href="https://www.sec.gov/data-research/sec-markets-data/information-about-registered-municipal-advisors" target="_blank">Information About Registered Municipal Advisors</a> — Names, SEC reporting file numbers, and CIK numbers for all registered municipal advisor firms.
- <a href="https://www.sec.gov/data-research/sec-markets-data/transfer-agent-data-sets" target="_blank">Transfer Agent Data Sets</a> — Registration and annual activities data for transfer agents (Forms TA-1, TA-2, TA-W). Updated quarterly.

## SEC — Other

- <a href="https://www.sec.gov/foia-services/frequently-requested-documents/foia-logs" target="_blank">FOIA Logs</a> — Freedom of Information Act request log files published by the SEC's Office of FOIA Services. Contains details on all FOIA requests submitted to the SEC since 2006, including requester type and subject.
  See <a href="https://doi.org/10.2308/TAR-2021-0146" target="_blank">Glaeser, Schonberger, Wasley, and Xiao (2023, <i>The Accounting Review</i>)</a> for an application studying private information acquisition via SEC FOIA requests.
  
## Python Tools for EDGAR

- <a href="https://github.com/john-friedman/datamule-python" target="_blank">datamule</a> <span class="badge badge-python">Python</span> <span class="badge badge-us">US</span> — Python package for downloading and processing SEC filings at scale. Supports batch downloads of any submission type (10-K, 10-Q, 8-K, Form 4, and more) by ticker or CIK. Free open-source core; optional cloud backend for faster bulk access without rate limits. By John Friedman. (<a href="https://pypi.org/project/datamule/" target="_blank">PyPI</a>)

```bash
pip install datamule
```

- <a href="https://github.com/jadchaar/sec-edgar-downloader" target="_blank">sec-edgar-downloader</a> <span class="badge badge-python">Python</span> <span class="badge badge-us">US</span> — Python library for bulk downloading SEC filings from EDGAR by ticker or CIK. Supports all filing types (10-K, 10-Q, 8-K, etc.) and saves filings to a structured local directory. (<a href="https://pypi.org/project/sec-edgar-downloader/" target="_blank">PyPI</a>)

```bash
pip install sec-edgar-downloader
```

## Firm Networks & Text-Based Data

- <a href="https://www.global-business-networks.com/" target="_blank">Global Business Networks</a> <span class="badge badge-csv">CSV</span> <span class="badge badge-global">Global</span> — Time-varying business network data for 63,000+ global firms, constructed using AI-generated business descriptions from 10-K filings (EDGAR) and international reports (LSEG). Includes networks based on Sentence-T5-XXL and OpenAI embedding models, plus masked variants to mitigate look-ahead bias. Coverage: 2000–2021. By Breitung & Müller (2025, *Journal of Financial Economics*). (<a href="https://data.mendeley.com/datasets/gdwm3m9xjz/1" target="_blank">Replication Data</a>)

---
**See also**: [Company Information](index.md) for annual reports, identifiers, and industry classification | [News & Media](../news-media/index.md) for Nexis Uni and news datasets | [WRDS](../../wrds/index.md) for Compustat and other database access.
