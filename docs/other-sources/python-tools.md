# Python Tools & Books

## Open-Source Tools by Jeroen Bouma (USE alumnus)

- <a href="https://www.jeroenbouma.com/projects/financetoolkit" target="_blank">Finance Toolkit</a> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> — An open-source Python toolkit for transparent financial analysis. Covers 150+ financial ratios, indicators, and performance measurements for equities, options, currencies, ETFs, indices, and more. Also includes economic indicators for 60+ countries. (<a href="https://github.com/JerBouma/FinanceToolkit" target="_blank">GitHub</a>)

```bash
pip install financetoolkit
```

- <a href="https://www.jeroenbouma.com/projects/financedatabase" target="_blank">Finance Database</a> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> — A database of 300,000+ financial symbols (equities, ETFs, funds, indices, currencies, cryptocurrencies, money markets) categorized by country, sector, and industry. Useful for identifying which products exist in a given market or industry. (<a href="https://github.com/JerBouma/FinanceDatabase" target="_blank">GitHub</a>)

```bash
pip install financedatabase
```

## Other Open-Source Tools

- <a href="https://pypi.org/project/yfinance/" target="_blank">yfinance</a> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> — Widely-used open-source Python library for downloading market data from Yahoo Finance. Covers historical prices, dividends, splits, fundamentals, options chains, and more for stocks, ETFs, mutual funds, currencies, and cryptocurrencies. (<a href="https://github.com/ranaroussi/yfinance" target="_blank">GitHub</a>)

```bash
pip install yfinance
```

- <a href="https://www.alphavantage.co/" target="_blank">Alpha Vantage</a> <span class="badge badge-api">API</span> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> — Free API providing historical and real-time market data for equities, forex, and cryptocurrencies, plus 50+ technical indicators and U.S. economic indicators. Free tier available (25 API calls/day); premium plans for higher rate limits. Requires a free API key. Python access via <a href="https://pypi.org/project/alpha-vantage/" target="_blank">`alpha-vantage`</a>. (<a href="https://github.com/RomelTorres/alpha_vantage" target="_blank">GitHub</a>)

```bash
pip install alpha-vantage
```

## Data Access

- <a href="https://pypi.org/project/pandas-datareader/" target="_blank">pandas-datareader</a> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> — Standard library for downloading economic and financial data into pandas DataFrames. Connects to FRED, World Bank, OECD, Eurostat, Yahoo Finance, and more. (<a href="https://github.com/pydata/pandas-datareader" target="_blank">GitHub</a>)

```bash
pip install pandas-datareader
```

- <a href="https://pypi.org/project/fredapi/" target="_blank">fredapi</a> <span class="badge badge-python">Python</span> <span class="badge badge-us">US</span> — Official Python wrapper for the FRED API, providing access to 800,000+ economic time series from the Federal Reserve Bank of St. Louis. Requires a free API key from <a href="https://fred.stlouisfed.org/docs/api/api_key.html" target="_blank">FRED</a>. (<a href="https://github.com/mortada/fredapi" target="_blank">GitHub</a>)

```bash
pip install fredapi
```

- <a href="https://pypi.org/project/wrds/" target="_blank">wrds</a> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> — Official WRDS Python connector for direct database access to Compustat, CRSP, and all WRDS datasets via SQL queries. Requires a WRDS account (available to UU students and staff). See also the [WRDS Python guide](../wrds/notebook.md).

```bash
pip install wrds
```

## Econometrics & Analysis

- <a href="https://pypi.org/project/linearmodels/" target="_blank">linearmodels</a> <span class="badge badge-python">Python</span> — Panel data models (fixed effects, random effects, between estimator), instrumental variables (2SLS, LIML, GMM), and system estimation. Standard package for applied finance research with panel data. (<a href="https://github.com/bashtage/linearmodels" target="_blank">GitHub</a>)

```bash
pip install linearmodels
```

- <a href="https://pypi.org/project/statsmodels/" target="_blank">statsmodels</a> <span class="badge badge-python">Python</span> — Time series analysis (ARIMA, VAR, VECM, GARCH via `arch`), hypothesis testing, OLS/WLS/GLS regression, and diagnostic tools. Foundation for econometric work in Python. (<a href="https://github.com/statsmodels/statsmodels" target="_blank">GitHub</a>)

```bash
pip install statsmodels
```

## Books

- <a href="https://www.tidy-finance.org/python/" target="_blank">Tidy Finance with Python</a> — Open-source textbook on empirical finance with Python, by Scheuch, Voigt, Weiss & Frey (Chapman & Hall/CRC). Covers tidy data principles, asset pricing (beta estimation, portfolio sorts, Fama-French factors), machine learning (ridge, lasso, random forests, neural networks), and portfolio optimization. Full book available free online. Also provides the <a href="https://github.com/tidy-finance/py-tidyfinance" target="_blank">`tidyfinance`</a> Python package with helper functions for downloading and preparing financial datasets.

!!! note
    Many examples in Tidy Finance use CRSP data, which Utrecht University does not have access to. The book's open-source data chapters and methodology sections remain fully usable.

---
**See also**: [Economic Data (with APIs)](economic-data.md) — the Finance Toolkit also covers economic indicators for 60+ countries.
