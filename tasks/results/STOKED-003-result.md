# Task Result: STOKED-003

**Status:** Completed ✅  
**Date:** 2026-04-24  
**Agent:** Dev

## Summary

Created and published the **Tops** collection on stoked-co.il Shopify store.

## Actions Taken

1. **Attempted to create** collection via `collectionCreate` mutation — collection already existed with handle `tops` (previously created).
2. **Updated description** to match spec exactly: *"Tees, hoodies, tanks and more — Stoked surf tops for every wave and every day."*
3. **Published** the collection to Online Store (Publication ID: `gid://shopify/Publication/64144375962`) via `publishablePublish` mutation.

## Final State

| Field        | Value |
|--------------|-------|
| ID           | `gid://shopify/Collection/358420185242` |
| Title        | Tops |
| Handle       | `tops` |
| Type         | Smart / Automatic |
| Rule         | TAG EQUALS `tops` |
| Description  | Tees, hoodies, tanks and more — Stoked surf tops for every wave and every day. |
| Published    | ✅ Yes (Online Store) |

## Acceptance Criteria

- [x] Collection exists with handle `tops`
- [x] Automatic rules filtering by tag `tops`
- [x] Published and visible on Online Store
