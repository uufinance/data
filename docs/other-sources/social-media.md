# Social Media Data

Repositories and platforms providing social media data for academic research. Access conditions vary — some data is freely downloadable, others require registration or approval.

!!! warning "Terms of Use & Research Ethics"
    Always review and comply with the terms of service of each platform before collecting or using data. Key considerations:

    - **Twitter/X**: The Developer Agreement prohibits redistribution of full tweet content; datasets are typically shared as Tweet IDs only, which must be "rehydrated" to obtain full content. Check the current [X Developer Agreement](https://developer.twitter.com/en/developer-terms/agreement-and-policy) for restrictions on commercial and academic use.
    - **Reddit**: The [Reddit API Terms](https://www.reddit.com/dev/api/) restrict large-scale scraping; use the official API and respect rate limits.
    - **Meta**: The [Meta Content Library](https://transparency.meta.com/researchtools/meta-content-library/) is only available to approved academic researchers.
    - **Privacy & consent**: Social media data often contains personal information. Consider GDPR obligations, IRB/ethics board requirements, and whether subjects could be re-identified from publicly posted content.
    - **Dynamic availability**: Platform API policies change frequently. Verify current access rules before building a research pipeline.

## Twitter / X

- <a href="https://github.com/shaypal5/awesome-twitter-data" target="_blank">Awesome Twitter Data</a> <span class="badge badge-global">Global</span> — Curated list of Twitter datasets and tools for research, including collections on elections, disasters, health, and financial topics.
- <a href="https://www.icpsr.umich.edu/web/pages/SOMAR/index.html" target="_blank">SOMAR — Social Media Archive at ICPSR</a> <span class="badge badge-global">Global</span> — Centralised repository for social media research data from large-scale platforms (Twitter, Facebook, Instagram, Reddit). Public datasets available for immediate download; restricted datasets accessible via a secure data enclave after approval. Maintained by the Inter-university Consortium for Political and Social Research (ICPSR).
- <a href="https://catalog.docnow.io/" target="_blank">DocNow Tweet Catalog</a> <span class="badge badge-global">Global</span> — Collectively curated listing of Twitter datasets shared as Tweet IDs, covering news events, social movements, and public discourse. Datasets can be rehydrated into full tweet records using the <a href="https://github.com/DocNow/hydrator" target="_blank">DocNow Hydrator</a> desktop application. Maintained by Documenting the Now.

## Meta (Facebook & Instagram)

- <a href="https://transparency.meta.com/researchtools/meta-content-library/" target="_blank">Meta Content Library</a> <span class="badge badge-global">Global</span> — Academic research tool providing access to public content from Facebook and Instagram (posts, comments, pages, groups). Requires application and approval by Meta for academic researchers. Access is via a secure research environment.

## Reddit

- <a href="https://www.reddit.com/dev/api/" target="_blank">Reddit API</a> <span class="badge badge-api">API</span> <span class="badge badge-global">Global</span> — Official REST API for accessing public posts, comments, subreddits, and user data. Free tier available; rate limits apply. Widely used in finance research for retail investor sentiment (e.g., WallStreetBets). Authentication via OAuth2.

## Other Platforms

- **LinkedIn**: No public research API. Academic data partnerships are handled case-by-case via [LinkedIn's Research Program](https://www.linkedin.com/help/linkedin/answer/a1341705).
- **YouTube**: The <a href="https://developers.google.com/youtube/v3" target="_blank">YouTube Data API v3</a> provides access to video metadata, comments, captions, and channel statistics. Free with a Google API key (subject to quota). Transcripts/captions can be retrieved programmatically and used for text analysis.
- **GitHub**: The <a href="https://docs.github.com/en/rest" target="_blank">GitHub REST API</a> and <a href="https://docs.github.com/en/graphql" target="_blank">GraphQL API</a> provide access to repository metadata, commit histories, issues, pull requests, and developer activity. Useful for research on open-source ecosystems, software development practices, and knowledge diffusion.

---
**See also**: [News & Media](news-media.md) for traditional news sources and Google Trends | [Sentiment & Culture](sentiment-culture.md) for text-based investor sentiment indices.
