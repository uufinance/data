# Audit Analytics

## Overview

Audit Analytics provides **audit, compliance, and governance data for SEC-registered companies**. The data is sourced from public filings (proxy statements, 10-K/10-Q filings, 8-K filings, etc.) and covers the US audit market comprehensively.

**What you can find here:**

- **Audit fees**: fees paid to external auditors for audit and non-audit services
- **Audit opinions**: going concern opinions, adverse opinions, and other audit report modifications
- **Auditor changes**: switches between audit firms, including reasons and timing
- **Financial restatements**: non-reliance (material) restatements of previously issued financial statements
- **Internal controls**: SOX 302 disclosure controls and SOX 404 internal control over financial reporting assessments
- **Director and officer changes**: CEO/CFO turnover and board member changes
- **Accelerated filer status**: SEC filing status classifications
- **Non-timely filers**: late filing notifications (NT 10-K, NT 10-Q)

Coverage starts from approximately **2000** for most datasets and includes all SEC registrants.

## WRDS Access

- **WRDS web interface**: <a href="https://wrds-www.wharton.upenn.edu/pages/get-data/audit-analytics/" target="_blank">Audit Analytics</a>
- **Python API libraries**: `audit_audit_comp`, `audit_common`
- **Update frequency**: Quarterly
- **Data dictionaries**:
    - <a href="https://wrds-www.wharton.upenn.edu/data-dictionary/audit_audit_comp/" target="_blank">Audit & Compliance</a>
    - <a href="https://wrds-www.wharton.upenn.edu/data-dictionary/audit_common/" target="_blank">Common</a>

## Key Tables

Use `conn.list_tables(library='audit_audit_comp')` and `conn.list_tables(library='audit_common')` in the Python API to see the full list of available tables.

### Audit & Compliance (`audit_audit_comp`)

| Table | Description | Use case |
|-------|-------------|----------|
| `feed03_audit_fees` | **Audit Fees** | Fees paid for audit, audit-related, tax, and other services. The most commonly used Audit Analytics table. |
| `feed05_audit_opinions` | **Audit Opinions** | Audit report details including going concern opinions and other modifications |
| `feed34_revised_audit_opinions` | **Revised Audit Opinions** | Changes or revisions to previously issued audit opinions |
| `feed02_auditor_changes` | **Auditor Changes** | Switches between audit firms, including reasons and dates |
| `feed01_auditors` | **Auditors** | Auditor firm information (name, location, PCAOB registration) |
| `feed07_current_auditor` | **Current Auditor** | The most recent auditor engagement for each company |
| `feed09_nonreliance_restatements` | **Non-Reliance Restatements** | Material restatements of previously issued financial statements (8-K Item 4.02) |
| `feed10_sox_302_disclosure_contro` | **SOX 302 Disclosure Controls** | Management's assessment of disclosure controls and procedures |
| `feed11_sox_404_internal_controls` | **SOX 404 Internal Controls** | Management and auditor assessments of internal control over financial reporting |
| `feed17_director_and_officer_chan` | **Director & Officer Changes** | CEO, CFO, and board member appointments and departures (8-K Item 5.02) |
| `feed16_accelerated_filer` | **Accelerated Filer** | SEC filing status classifications (large accelerated, accelerated, non-accelerated, smaller reporting) |
| `feed20_nt` | **Non-Timely Filer** | Late filing notifications (NT 10-K, NT 10-Q) |
| `feed06_benefit_plan_opinions` | **Benefit Plan Opinions** | Audit opinions on employee benefit plans |

### Common (`audit_common`)

The `audit_common` library contains shared reference and lookup tables used across Audit Analytics modules. Use `conn.list_tables(library='audit_common')` to explore its contents.

## Linking to Compustat and CRSP

Audit Analytics identifies companies using the SEC's **CIK** (Central Index Key). To link with Compustat or CRSP, match on `company_fkey` (CIK) from Audit Analytics to `cik` in Compustat's `company` table, or use the WRDS linking tables.

## Example: Querying Audit Fees

```python
import wrds
conn = wrds.Connection()

# List available tables in Audit & Compliance
conn.list_tables(library='audit_audit_comp')

# Get audit fees for recent fiscal years
audit_fees = conn.raw_sql("""
    SELECT company_fkey, fiscal_year, audit_fees, auditor_name
    FROM audit_audit_comp.feed03_audit_fees
    WHERE fiscal_year >= 2019
""")
```

## Example: Querying Non-Reliance Restatements

```python
# Get all non-reliance restatements since 2019
restatements = conn.raw_sql("""
    SELECT company_fkey, file_date, res_begin_date, res_end_date,
           res_accounting, res_fraud, res_sec_invest
    FROM audit_audit_comp.feed09_nonreliance_restatements
    WHERE file_date >= '2019-01-01'
""")
```

> **Tip**: Table names on WRDS may change over time. Always run `conn.list_tables(library='audit_audit_comp')` to verify the current table names, and use `conn.describe_table(library='audit_audit_comp', table='<table_name>')` to inspect available columns before querying.

For more examples, see the [Python API notebook](../notebook.md).
