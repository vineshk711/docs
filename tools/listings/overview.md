---
title: "Listings Overview"
description: "Tools for managing and analyzing your business listings across Google, Facebook, Bing, Apple, and other platforms."
---

## Tools in this category

- [get\_listing](get-listing.md) — Full listing profile for a single location — hours, categories, photos, per-site status
- [get\_listing\_location\_status\_report](get-listing-location-status-report.md) — Synced/Submitted/Action Required counts for all listing sites at a location
- [get\_listing\_insights](get-listing-insights.md) — Aggregated Google (and other) listing analytics — map views, calls, directions, website visits
- [get\_listing\_category\_list](get-listing-category-list.md) — Available listing categories for a given site (Google, Bing, Facebook, etc.) and country
- [get\_product\_listing\_list](get-product-listing-list.md) — Google Merchant product listings linked to your account

## Location-Level Tools

{% hint style="warning" %}
`get_listing` and `get_listing_location_status_report` are **location-level tools** — they require a `locationId` parameter.

Call [get\_child\_locations](../business/get-child-locations.md) first to get the list of valid location IDs.
{% endhint %}

## Tips

- `get_listing_insights` defaults to the last 12 months if no date range is provided.
- `get_listing_category_list` is useful before updating a listing — use it to find the correct category ID for a given platform.
- `get_product_listing_list` only returns data if your Google Merchant account is connected in Birdeye.
