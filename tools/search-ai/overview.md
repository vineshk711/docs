---
title: "Search AI Overview"
description: "Tools for tracking how AI engines like ChatGPT, Gemini, and Perplexity represent your business."
---

## What is Search AI?

Search AI is Birdeye's capability to monitor how AI-powered search engines and chatbots (ChatGPT, Gemini, Perplexity) respond to prompts about your business category. It tracks:

- Which URLs those AI engines cite when answering
- Which businesses they surface in their answers
- How accurately they report your business information (NAP accuracy)
- How they characterize your business (SWOT/sentiment)

## Tools in this category

- [get\_search\_ai\_configuration](get-search-ai-configuration.md) — View Search AI themes and the exact prompts being monitored
- [get\_search\_ai\_available\_runs](get-search-ai-available-runs.md) — See past Search AI run dates and which themes were analyzed
- [get\_search\_ai\_citations](get-search-ai-citations.md) — URLs cited by ChatGPT, Gemini, or Perplexity when answering your prompts
- [get\_search\_ai\_businesses](get-search-ai-businesses.md) — Businesses that AI engines surface in response to your monitored prompts
- [get\_search\_ai\_accuracy\_report](get-search-ai-accuracy-report.md) — NAP accuracy — how correctly AI engines report your name, address, phone, hours, and website
- [get\_search\_ai\_sentiment\_report](get-search-ai-sentiment-report.md) — SWOT analysis — Strengths, Weaknesses, Opportunities, and Threats as perceived by AI engines

## Supported AI Models

| Value | AI Engine |
|---|---|
| `CHATGPT` | OpenAI ChatGPT |
| `GEMINI` | Google Gemini |
| `PERPLEXITY` | Perplexity AI |

## Tips

- Start with `get_search_ai_configuration` to understand which themes and prompts are being tracked.
- Call `get_search_ai_available_runs` to find valid date ranges before querying reports.
- Use `get_search_ai_accuracy_report` with specific `businessNumbers` (location IDs) for per-location NAP accuracy.
