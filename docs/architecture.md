# Stoked AI System — Architecture

## Overview
A fully autonomous multi-agent system controlling the Stoked Shopify store.

## Command Flow
```
Zion (WhatsApp)
    ↓
CEO Agent
    ↓
[Dev Team | Marketing Team | Support Team]
    ↓
GitHub / Shopify / Printify / Ad Platforms
```

## Data Flow
```
Shopify + Printify → BI Agent → Analytics Agent → Campaign Agent
                                                 → Budget Guardian
                                                 → Dev PM Agent
```

## Deployment Flow
```
CEO → PM → Developer → QA → DevOps → GitHub Actions → Shopify
```

## Integration Map
| Platform   | Agent(s) Using It         |
|------------|---------------------------|
| Shopify    | DevOps, Support, Analytics|
| Printify   | Developer, Support        |
| GitHub     | Developer, QA, DevOps     |
| Meta       | Campaign                  |
| Google Ads | Campaign                  |
| TikTok     | Campaign                  |
| Klaviyo    | Email/SMS                 |
| WhatsApp   | CEO (command interface)   |
