---
title: Battlenet
sidebarTitle: Battlenet
---

API configuration: `battlenet`

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the community.

## Getting started

-   [How to register an Application](https://develop.battle.net/documentation/guides/getting-started)
-   [OAuth-related docs](https://develop.battle.net/documentation/guides/using-oauth)
-   [List of OAuth scopes](https://develop.battle.net/documentation/guides/using-oauth#:~:text=Scopes%20and%20OAuth%20enabled%20APIs)

Do you need help? Please check this link.

## Connection configuration in Terapi

Battlenet uses different domain extensions for different regions.

You need to pass the domain extension to use to Terapi in the `terapi.auth()` call:

```js
terapi.auth('battlenet', '', });
```

Add Connection configuration in Terapi by editing this page.
    
