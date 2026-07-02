---
title: "Reviews Overview"
description: "Tools for accessing review data, rating trends, and per-source summaries."
---

## Tools in this category

- [review\_and\_rating\_overview](review-and-rating-overview.md) — Get aggregated review volume and rating trends over a date range
- [get\_reviews](get-reviews.md) — Fetch individual reviews with full detail — rating, comment, reviewer info, source, status
- [get\_review\_summary](get-review-summary.md) — Get total review counts and average ratings grouped by review source

## Tips

- All three tools operate at the account level — no `locationId` needed.
- Use `review_and_rating_overview` for trend analysis and `get_review_summary` for per-platform breakdowns.
- Use `get_reviews` when you need the actual review text or want to filter by rating, source, or status.
