# Cryptocurrency & Digital Asset Data

Free and open-access data sources for cryptocurrency market prices, on-chain metrics, and exchange data.

!!! tip
    Most free-tier crypto APIs have rate limits or limited history. For academic research requiring long, clean time series, CoinGecko and CryptoCompare are the most commonly used free sources.

## Market Price Data

- <a href="https://www.coingecko.com/en/api" target="_blank">CoinGecko API</a> <span class="badge badge-api">API</span> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> <span class="badge badge-crypto">Crypto</span> — Free API for current and historical cryptocurrency market data, including prices, market cap, trading volume, and exchange data for 10,000+ coins. Historical OHLCV data available. Free tier supports 10,000–30,000 calls/month; no API key required for basic access. Python access via <a href="https://pypi.org/project/pycoingecko/" target="_blank">`pycoingecko`</a>. (<a href="https://github.com/man-c/pycoingecko" target="_blank">GitHub</a>)

```bash
pip install pycoingecko
```

- <a href="https://min-api.cryptocompare.com/" target="_blank">CryptoCompare API</a> <span class="badge badge-api">API</span> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> <span class="badge badge-crypto">Crypto</span> — Historical and real-time OHLCV data for cryptocurrencies across 250+ exchanges. Free tier provides access to daily, hourly, and minute-level data with up to 2,000 data points per request. API key required (free registration). Widely used in academic research for constructing crypto price panels.

- <a href="https://www.cryptodatadownload.com/" target="_blank">Crypto Data Download</a> <span class="badge badge-csv">CSV</span> <span class="badge badge-global">Global</span> <span class="badge badge-crypto">Crypto</span> — Free historical OHLCV data for major cryptocurrencies across leading exchanges (Binance, Coinbase, Kraken, Bitstamp, and others), available as direct CSV downloads. No registration required. Covers daily and hourly data.

## Exchange & Trading Data

- <a href="https://github.com/ccxt/ccxt" target="_blank">CCXT</a> <span class="badge badge-api">API</span> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> <span class="badge badge-crypto">Crypto</span> — Open-source Python/JavaScript/PHP library providing a unified interface to 100+ cryptocurrency exchange APIs. Supports fetching order books, OHLCV data, trades, balances, and more. The standard tool for programmatic access to live and historical crypto exchange data. (<a href="https://pypi.org/project/ccxt/" target="_blank">PyPI</a>)

```bash
pip install ccxt
```

- <a href="https://data.binance.vision/" target="_blank">Binance Public Data</a> <span class="badge badge-csv">CSV</span> <span class="badge badge-global">Global</span> <span class="badge badge-crypto">Crypto</span> — Free bulk downloads of historical trading data from Binance, the world's largest crypto exchange by volume. Covers klines (OHLCV), trades, and aggregate trades at tick, minute, hourly, and daily frequencies. Data available from 2017 onwards. No registration required.

## On-Chain & Blockchain Data

- <a href="https://blockchair.com/api" target="_blank">Blockchair API</a> <span class="badge badge-api">API</span> <span class="badge badge-global">Global</span> <span class="badge badge-crypto">Crypto</span> — Universal blockchain explorer and search engine with a free API covering Bitcoin, Ethereum, and 40+ other blockchains. Provides transaction data, address balances, block data, and mempool statistics. Free tier available with rate limits.

- <a href="https://www.blockchain.com/explorer/api/blockchain_api" target="_blank">Blockchain.com API</a> <span class="badge badge-api">API</span> <span class="badge badge-global">Global</span> <span class="badge badge-crypto">Crypto</span> — Free API for Bitcoin blockchain data including transaction details, block data, address balances, and aggregate market statistics. Provides summary statistics on hash rate, difficulty, and mempool. No API key required for basic endpoints.

---
**See also**: [Python Tools & Books](python-tools.md) for yfinance (covers crypto via Yahoo Finance) and Alpha Vantage (covers crypto market data).
