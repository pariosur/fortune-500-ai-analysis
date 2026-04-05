# Fortune 500 AI Mentions in SEC 10-K Filings (2022–2025)

Dataset tracking AI and Generative AI mentions in SEC 10-K filings across the Fortune 500 from 2022 to 2025.

## Summary

| Year | Total Companies | With AI | % With AI | Total Mentions | Risk | Benefit | Both |
|------|-----------------|---------|-----------|----------------|------|---------|------|
| 2022 | 500 | 144 | 28.8% | 1,157 | 17 | 43 | 84 |
| 2023 | 500 | 165 | 33.0% | 1,647 | 22 | 46 | 97 |
| 2024 | 500 | 345 | 69.0% | 5,101 | 86 | 22 | 237 |
| 2025 | 500 | 423 | 84.6% | 8,105 | 75 | 18 | 330 |

## Files

- `fortune500_ai_mentions_2022.csv`
- `fortune500_ai_mentions_2023.csv`
- `fortune500_ai_mentions_2024.csv`
- `fortune500_ai_mentions_2025.csv`

## Data Dictionary

| Column | Description |
|--------|-------------|
| Rank | Fortune 500 rank by revenue |
| Company Name | Company name |
| Ticker | Stock ticker symbol |
| Status | AI mention status: `Mentions AI` or `No AI Mention` |
| Sector | Industry sector |
| Subsector | Industry subsector |
| Filing Date | 10-K filing date |
| Revenue Millions | Annual revenue in millions USD |
| Revenue Growth Pct | Year-over-year revenue growth |
| AI Mentions | Total count of AI-related terms |
| GenAI Mentions | Count of generative AI-specific terms |
| Classification | `Risk`, `Benefit`, `Both`, or `No AI Mention` |

## Methodology

**Data Source:** SEC 10-K/20-F filings for Fortune 500 companies, fiscal years 2022–2025, downloaded from EDGAR and processed through [Metal](https://metal.ai).

**AI Terms searched** (regex, case-insensitive):
- "artificial intelligence"
- "A.I." / "AI" (standalone, with or without periods)
- "machine learning" (standalone "ML" excluded due to false positives)
- "deep learning"
- "neural network"

**GenAI Terms searched** (regex, case-insensitive):
- "generative AI" / "GenAI" / "generative artificial intelligence"
- "LLM" / "large language model"
- "GPT" / "ChatGPT"

**Mention Counting:** Regex-based search across full filing text. Each mention was mapped to its 10-K section (e.g., Item 1 Business, Item 1A Risk Factors, Item 7 MD&A) via section header parsing.

**Classification:** An LLM-powered workflow classified each company as `Risk`, `Benefit`, `Both`, or `No AI Mention` based on the filing content, and extracted representative quotes for each category.

## Analysis

Full analysis with charts and insights: [Fortune 500 AI Disclosure Analysis](https://dev.to/riospablo/fortune-500-ai-disclosure-analysis-how-americas-largest-companies-talk-about-ai-in-sec-filings-5531)

## License

This dataset is released under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the data with attribution.

## Author

[Pablo Rios](https://github.com/pariosur) 