# WRDS (Wharton Research Data Services)

## How to Get a WRDS Account

In order to use WRDS, you need to register for an account on the WRDS website. Opening a new account is simple and requires only a couple of minutes.

### Step 1: Go to the WRDS Website

Navigate to <a href="https://wrds-www.wharton.upenn.edu/" target="_blank">https://wrds-www.wharton.upenn.edu/</a> and click on the **Register** button.

### Step 2: Select Your Institution

In the first menu, select your university. For students of Utrecht University, select **Utrecht University**.

### Step 3: Choose Your Affiliation

For **Affiliation with Institution**, select the option that best fits your role (e.g., Undergraduate, Masters, PhD, Faculty).

### Step 4: Complete the Registration Form

Fill in the required details. Note that **usernames are permanent** and cannot be modified once you have requested your account. Check with your institution's representative if there are any username requirements before creating your account.

### Step 5: Wait for Approval

After submitting your registration, you will receive an email with login instructions once the WRDS administrators approve your request. Approval may take up to 48 hours.

### Important Notes

- The default expiration for student accounts is **2 years**.
- WRDS policy prohibits undergraduate/master's students from accessing WRDS during the extended break between semesters. Accounts are temporarily disabled during this time and automatically re-enabled when the new semester begins.
- If you need access to a specific database or have questions, send an email to **financedata.use@uu.nl** with your name, position/degree programme (BSc/MSc), type of data required, and details of your request.

### Getting Help

- For support, click on **Support** > **Contact WRDS Support** on the WRDS website and fill out the form.

## Accessing Data via the Python API

See the **[Basics of Using Python on WRDS Platform](Basics%20of%20Using%20Python%20on%20WRDS%20Platform.ipynb)** notebook for a hands-on guide covering:

- Installing and connecting to WRDS with Python
- Listing available databases and tables
- Querying data with SQL
- Joining multiple datasets
- Exporting results to CSV, Excel, Stata, and pickle

For a full overview of all variables and tables, see the <a href="https://wrds-www.wharton.upenn.edu/data-dictionary/data-dictionary/" target="_blank">WRDS Data Dictionary</a>.

## Databases

### Paid Subscriptions

Utrecht University has paid subscriptions to the following databases. Click the guide link for details on available tables, API library names, and what data you can expect to find.

| Database | Description | Guide |
|----------|-------------|-------|
| **Compustat North America** | Corporate fundamental financial data (income statement, balance sheet, cash flow) and stock prices for US and Canadian companies | [Guide](databases/compustat-north-america.md) |
| **Compustat Bank** | Fundamental financial data for North American banks and financial institutions | [Guide](databases/compustat-bank.md) |
| **Compustat Global** | Global company fundamentals, stock prices, exchange rates, and index data (80+ countries) | [Guide](databases/compustat-global.md) |
| **ExecuComp** | Executive and director compensation data for S&P 1500 companies | [Guide](databases/execucomp.md) |
| **Compustat Historical Segments** | Business and geographic segment-level data (revenue, assets by segment) | [Guide](databases/compustat-segments.md) |
| **Mergent FISD** | Fixed income securities: bond issue details, issuer information, credit ratings | [Guide](databases/mergent-fisd.md) |

### Additional Free Data

Next to paid subscriptions, WRDS offers additional free data, including contributed data used in publications by researchers. For example:

- <a href="https://wrds-www.wharton.upenn.edu/pages/get-data/otc-corporate-bond-and-agency-debt-bond-transaction-data/trace-enhanced/bond-trades/" target="_blank">TRACE</a>: bond market transactions
- <a href="https://wrds-www.wharton.upenn.edu/pages/get-data/wrds-bond-returns/wrds-bond-returns/" target="_blank">Bond Returns</a> and <a href="https://wrds-www.wharton.upenn.edu/pages/get-data/otc-markets-group/" target="_blank">OTC Markets</a>
- <a href="https://wrds-www.wharton.upenn.edu/pages/get-data/subsidiary-data-wrds/" target="_blank">Subsidiary Data</a>
- <a href="https://wrds-www.wharton.upenn.edu/pages/get-data/wrds-us-patents/" target="_blank">US Patents</a>
- <a href="https://wrds-www.wharton.upenn.edu/pages/get-data/world-indices-wrds/" target="_blank">World Indices</a>
- <a href="https://wrds-www.wharton.upenn.edu/pages/get-data/historical-sp-dow-jones-indices-spdji/" target="_blank">S&P Dow Jones Indices</a>

Find out yourself which module is useful.
