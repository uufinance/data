# News

Data sources for news content, media coverage, and online search trends. For social media platforms, see [Social Media](../social-media.md).

- <a href="https://databanken.library.uu.nl/nexis-uni" target="_blank">Nexis Uni</a> <span class="badge badge-global">Global</span> — Full text of articles from Dutch and international newspapers and news magazines. Also provides company information on Dutch and international businesses, and Market Insight. Accessible to UU students and staff via the Utrecht University Library.
- <a href="https://structureofnews.com/" target="_blank">Structure of News</a> <span class="badge badge-csv">CSV</span> <span class="badge badge-global">Global</span> — Structured dataset mapping the topics, sources, and formats found in news journalism across countries and outlets. Designed for computational analysis of news content and media diversity. Useful for studying media framing, information dissemination, and coverage patterns in financial markets research.
- <a href="https://trends.google.com/trends/" target="_blank">Google Trends</a> <span class="badge badge-api">API</span> <span class="badge badge-global">Global</span> — Relative search interest over time for any query, by country, region, and category. Widely used as a real-time proxy for investor attention, household financial concerns, and information demand. Data is normalised (0–100 within each query). Accessible via the website or programmatically with the <a href="https://pypi.org/project/pytrends/" target="_blank">`pytrends`</a> Python library.
- <a href="https://www.mediawiki.org/wiki/Wikimedia_REST_API" target="_blank">Wikimedia REST API</a> <span class="badge badge-api">API</span> <span class="badge badge-python">Python</span> <span class="badge badge-global">Global</span> — Free API providing daily and monthly page view counts for any Wikipedia article across all language editions, from 2015 to present. Useful as a proxy for public interest and attention — covering companies, industries, events, and topics. No authentication required. Accessible via the <a href="https://wikimedia.org/api/rest_v1/#/Pageviews_data" target="_blank">Pageviews endpoint</a> or with the <a href="https://pypi.org/project/pageviewsapi/" target="_blank">`pageviewsapi`</a> Python package.

```bash
pip install pageviewsapi
```

---
**See also**: [Social Media](../social-media.md) for platform data (Twitter/X, Reddit, Meta) | [Sentiment & Culture](../sentiment-culture.md) for text-based sentiment indices | [Company Filings (SEC EDGAR)](../company-info-news.md) for EDGAR full-text search.
