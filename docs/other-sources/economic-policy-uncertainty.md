# Economic Policy Uncertainty Indices <span class="badge badge-csv">CSV</span> <span class="badge badge-fred">FRED</span> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span>

The <a href="https://www.policyuncertainty.com/" target="_blank">policyuncertainty.com</a> website, maintained by Scott R. Baker, Nick Bloom, and Steven J. Davis, hosts a large collection of text-based uncertainty and risk indices. All indices are newspaper-based (or text-based) and freely downloadable. Many are also available via <a href="https://fred.stlouisfed.org/categories/33446" target="_blank">FRED</a>. Data is licensed under <a href="https://creativecommons.org/licenses/by/4.0/" target="_blank">CC BY 4.0</a>.

---

## Economic Policy Uncertainty (EPU)

The headline index quantifies economic policy uncertainty by counting newspaper articles that contain terms related to the economy, policy, and uncertainty.

| Variant | Coverage | Frequency | Period |
|---------|----------|-----------|--------|
| <a href="https://www.policyuncertainty.com/us_monthly.html" target="_blank">US EPU</a> | United States (10 newspapers) | Monthly, daily | 1985–present |
| <a href="https://www.policyuncertainty.com/all_country_data.html" target="_blank">Country-level EPU</a> | 25+ countries | Monthly | varies by country |
| <a href="https://www.policyuncertainty.com/global_monthly.html" target="_blank">Global EPU (GEPU)</a> | GDP-weighted average of 18 national indices | Monthly | 1997–present |
| <a href="https://www.policyuncertainty.com/categorical_epu.html" target="_blank">US Categorical EPU</a> | Policy sub-categories (see below) | Monthly | 1985–present |

The US categorical EPU breaks down uncertainty by policy domain — for example, monetary policy, fiscal policy, healthcare, trade policy, national security, and more. Each sub-index adds category-specific search terms on top of the baseline economy-uncertainty-policy filter.

!!! tip "Use in finance"
    The EPU index is widely used as a control variable or main explanatory variable in studies on investment, asset pricing, corporate decisions, and macro-finance. It is available on FRED as <a href="https://fred.stlouisfed.org/series/USEPUINDXM" target="_blank">`USEPUINDXM`</a> (monthly) and <a href="https://fred.stlouisfed.org/series/USEPUINDXD" target="_blank">`USEPUINDXD`</a> (daily).

**Key reference**: Baker, S.R., Bloom, N. and Davis, S.J. (2016). Measuring Economic Policy Uncertainty. *The Quarterly Journal of Economics*, 131(4), 1593–1636. <a href="https://doi.org/10.1093/qje/qjw024" target="_blank">doi:10.1093/qje/qjw024</a>

---

## Geopolitical Risk (GPR)

The <a href="https://www.policyuncertainty.com/gpr.html" target="_blank">Geopolitical Risk Index</a> by Caldara and Iacoviello counts newspaper articles related to adverse geopolitical events across 10 international newspapers, organized into eight categories (war threats, military buildups, nuclear threats, terror threats, and actual geopolitical acts).

| Variant | Coverage | Frequency | Period |
|---------|----------|-----------|--------|
| GPR Benchmark | 10 newspapers | Monthly, daily | 1985–present |
| GPR Historical (GPRH) | 3 newspapers | Monthly | 1900–present |
| Geopolitical Threats (GPRT) | Threat categories 1–5 | Monthly | 1985–present |
| Geopolitical Acts (GPRA) | Act categories 6–8 | Monthly | 1985–present |
| Country-specific GPR | 44 countries | Monthly | varies |

!!! tip "Use in finance"
    The GPR index is used in studies on risk premia, flight-to-safety, capital flows, and investment under uncertainty. Higher GPR foreshadows lower investment and employment and is associated with larger downside risks.

**Key reference**: Caldara, D. and Iacoviello, M. (2022). Measuring Geopolitical Risk. *American Economic Review*, 112(4), 1194–1225. <a href="https://doi.org/10.1257/aer.20191823" target="_blank">doi:10.1257/aer.20191823</a>

---

## World Uncertainty Index (WUI)

The <a href="https://www.policyuncertainty.com/wui_quarterly.html" target="_blank">World Uncertainty Index</a> by Ahir, Bloom, and Furceri counts the frequency of "uncertainty" in the Economist Intelligence Unit (EIU) country reports for 143 countries (covering 99% of world GDP).

| Variant | Coverage | Frequency | Period |
|---------|----------|-----------|--------|
| WUI | 143 countries | Quarterly | 1952–present |
| World Trade Uncertainty (WTU) | 143 countries | Quarterly | 1996–present |

!!! tip "Use in finance"
    The WUI provides broad cross-country coverage and is well suited for panel studies on uncertainty and economic outcomes. Available on FRED as <a href="https://fred.stlouisfed.org/series/WUIGLOBALWEIGHTAVG" target="_blank">`WUIGLOBALWEIGHTAVG`</a>.

**Key reference**: Ahir, H., Bloom, N. and Furceri, D. (2022). The World Uncertainty Index. NBER Working Paper 29763. <a href="https://www.nber.org/papers/w29763" target="_blank">nber.org/papers/w29763</a>

---

## Monetary Policy Uncertainty (MPU)

| Variant | Coverage | Frequency | Period |
|---------|----------|-----------|--------|
| <a href="https://www.policyuncertainty.com/bbd_monetary.html" target="_blank">Baker-Bloom-Davis MPU</a> | United States | Monthly | 1985–present |
| <a href="https://www.policyuncertainty.com/monetary.html" target="_blank">Husted-Rogers-Sun MPU</a> | United States | Monthly | 1985–present |
| Arbatli et al. MPU | Japan | Monthly | 1987–present |

---

## Trade Policy Uncertainty

| Variant | Coverage | Frequency | Period |
|---------|----------|-----------|--------|
| <a href="https://www.policyuncertainty.com/trade_uncertainty.html" target="_blank">BBD Trade Policy Uncertainty</a> | United States | Daily | 1985–present |
| <a href="https://www.policyuncertainty.com/trade_cimpr.html" target="_blank">Caldara et al. Trade Policy Uncertainty</a> | United States | Monthly | 1960–present |

---

## Equity Market Volatility (EMV) Trackers

Newspaper-based trackers of equity market volatility that move closely with the VIX.

| Variant | Coverage | Frequency | Period |
|---------|----------|-----------|--------|
| <a href="https://www.policyuncertainty.com/EMV_monthly.html" target="_blank">Overall EMV</a> | United States | Monthly, daily | 1985–present |
| <a href="https://www.policyuncertainty.com/infectious_EMV.html" target="_blank">Infectious Disease EMV</a> | United States | Daily | 1985–present |
| 40+ categorical EMV trackers | United States | Monthly | 1985–present |

**Key reference**: Baker, S.R., Bloom, N., Davis, S.J. and Kost, K. (2019). Policy News and Stock Market Volatility. NBER Working Paper 25720.

---

## Climate & Sustainability

| Variant | Coverage | Frequency | Period |
|---------|----------|-----------|--------|
| <a href="https://www.policyuncertainty.com/climate_uncertainty.html" target="_blank">Climate Policy Uncertainty (CPU)</a> | United States | Monthly | 1985–present |
| US Climate Uncertainty | United States | Monthly | varies |
| Sustainability Uncertainty | United States | Monthly | varies |

---

## Other Specialized Indices

The site also hosts indices on:

- **AI Economic Uncertainty** — newspaper-based index tracking uncertainty related to artificial intelligence
- **US-China Tension Index** — measures bilateral geopolitical and economic tensions
- **Inter-Korean Geopolitical Risk** — Korea-specific GPR
- **Cable News-based EPU** — EPU derived from cable news transcripts
- **Twitter-based Uncertainty** — social-media-based uncertainty measures
- **Energy Uncertainty Indexes** — energy-sector-specific uncertainty
- **Financial Stress Indicator** — newspaper-based financial stress
- **Firm-Level Political Risk** — firm-level measures from earnings calls (Hassan et al.)
- **Immigration-Related Indices** — immigration policy uncertainty

---

## Python Example

Many indices are available via FRED:

```python
from fredapi import Fred
fred = Fred(api_key="your_key")

# US Economic Policy Uncertainty (monthly)
epu = fred.get_series("USEPUINDXM")

# Global EPU (GDP-weighted)
gepu = fred.get_series("GEPUCURRENT")

# World Uncertainty Index (GDP-weighted)
wui = fred.get_series("WUIGLOBALWEIGHTAVG")
```

Or download directly from the website:

```python
import pandas as pd

# US monthly EPU
url = "https://www.policyuncertainty.com/media/US_Policy_Uncertainty_Data.xlsx"
epu = pd.read_excel(url)
```

---
**See also**: [Sentiment & Culture](sentiment-culture.md) for investor sentiment surveys, cultural dimensions, and values surveys.
