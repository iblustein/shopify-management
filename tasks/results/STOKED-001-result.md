# Task Result: STOKED-001

## Status: Completed

## Task
Create the All Products smart collection on Shopify for stoked.co.il.

## What Was Done
- Created a Smart Collection (automatic) via Shopify GraphQL API (collectionCreate mutation)
- Title: All Products
- Handle: all
- Description: Shop the full Stoked catalog — surf lifestyle apparel and accessories.
- Collection ID: gid://shopify/Collection/358420021402
- Rule Set: appliedDisjunctively: false, rule: TITLE NOT_EQUALS "ZZZZZ_NOMATCH" — standard Shopify pattern to include all products automatically (Shopify GraphQL does not support a native status=active smart rule; this catch-all rule includes all products, and only active/published products surface on storefront)

## Verification
- Collection confirmed live with handle: all
- Description confirmed set correctly
- Products pulling in: YES (e.g. Unisex Oversized Boxy Tee — status: ACTIVE)
- Collection is published and visible

## Notes
Shopify GraphQL Admin API does not expose a PRODUCT_STATUS column for smart collection rules. The standard approach for an all-products collection is a catch-all rule (title not equals a nonsense string), which effectively includes all active products in the storefront context.

## Date
2026-04-24
