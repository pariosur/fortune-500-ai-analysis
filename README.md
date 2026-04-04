# Fortune 500 AI Mentions (2022–2025)

Dataset tracking AI mentions in SEC 10-K filings across the Fortune 500 from 2022 to 2025.

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
| Classification | `Risk`, `Benefit`, or `Both` |

## Methodology

**Data Source:** SEC 10-K filings for Fortune 500 companies, fiscal years 2022–2025

**AI Terms:** "artificial intelligence," "machine learning," "deep learning," "neural network"

**GenAI Terms:** "generative AI," "generative artificial intelligence," "LLM," "large language model," "GPT"

**Classification:** Companies were classified based on whether AI appears in risk factor sections only, business/opportunity sections only, or both.

## Analysis

Full analysis with charts and insights: [dev.to/pariosur](https://dev.to/pariosur) *(coming soon)*

## License

This dataset is released under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the data with attribution.

## Author

[Pablo Rios](https://github.com/pariosur) · [Metal](https://metal.ai)
