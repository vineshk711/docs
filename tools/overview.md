---
title: "Tools Overview"
description: "Birdeye MCP provides a variety of read-only tools across different categories. All tools use your authenticated Birdeye account context"
---

## Tool Categories

- [Reviews](reviews/overview.md) — Review trends, rating overviews, and individual review data
- [Business](business/get-business-info.md) — Business profile and child location discovery
- [Surveys](surveys/get-all-surveys.md) — Survey catalog and paginated response data
- [Listings](listings/overview.md) — Listing profiles, status reports, insights, and product listings
- [Search AI](search-ai/overview.md) — AI engine citations, business visibility, accuracy, and SWOT reports
- [Social](social/track-social-post.md) — Social performance reports across multiple channels like Instagram, Facebook, LinkedIn etc.
- [Ticketing](ticketing/get-all-ticket-data.md) — Ticket retrieval with filtering and pagination
- [Aggregation](aggregation/get-all-aggregation-sources.md) — Review source monitoring and site alias lookup

## All Tools

| Tool | Module | Description |
|---|---|---|
| `review_and_rating_overview` | Reviews | Review and rating trends over a time period |
| `get_reviews` | Reviews | Individual reviews with full details |
| `get_review_summary` | Reviews | Review counts and averages grouped by source |
| `get_business_info` | Business | Business profile of the authenticated user |
| `get_child_locations` | Business | All child locations of the enterprise account |
| `get_all_surveys` | Surveys | All surveys for the business |
| `get_survey_responses` | Surveys | Paginated responses for a specific survey |
| `get_listing` | Listings | Full listing profile for a single location |
| `get_listing_location_status_report` | Listings | Listing sync status across sites for a location |
| `get_listing_insights` | Listings | Google and other listing analytics |
| `get_listing_category_list` | Listings | Available listing categories by source and country |
| `get_product_listing_list` | Listings | Google Merchant product listings |
| `get_search_ai_configuration` | Search AI | Search AI themes and prompt configuration |
| `get_search_ai_available_runs` | Search AI | Past Search AI run dates and themes |
| `get_search_ai_citations` | Search AI | URLs cited by AI engines (ChatGPT, Gemini, Perplexity) |
| `get_search_ai_businesses` | Search AI | Businesses surfaced by AI engines for your prompts |
| `get_search_ai_accuracy_report` | Search AI | NAP accuracy as reported by AI engines |
| `get_search_ai_sentiment_report` | Search AI | SWOT analysis from AI engine sentiment |
| `track_social_post` | Social | Status and metrics for a published social post |
| `get_social_open_url_performance_report` | Social | Channel-level social performance with comparison |
| `get_all_ticket_data` | Ticketing | Tickets with full filtering and pagination |
| `get_all_aggregation_sources` | Aggregation | Review monitoring URLs configured for the business |
| `get_review_site_aliases` | Aggregation | Review site aliases configured for the business |

## Common Patterns

### Enterprise Accounts with Multiple Locations

Most tools operate at the **account level** automatically. For tools that require a specific location (marked as **location-level**), first call `get_child_locations` to retrieve valid `locationId` values.

```
1. get_child_locations          → get list of {id, name} for each location
2. get_listing(locationId=...)  → use a location id from step 1
```
