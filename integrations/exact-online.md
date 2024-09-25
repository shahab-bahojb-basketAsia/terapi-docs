---
title: Exact Online
sidebarTitle: Exact Online
---

API Configuration: `exact-online`

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

-   Register your app on the [Exact Online Developer Portal](https://apps.exactonline.com/)
-   Terapi supports the [Authorization Web APIs](https://support.exactonline.com/community/s/knowledge-base#All-All-DNO-Content-gettingstarted) for implementing the `authorization code` flow.

Need help getting started? Get help in the community.

## Connection configuration in Terapi

Exact Online uses region-specific domain extensions.

You need to pass the region's domain extension to Terapi in the `terapi.auth()` call:

```js
terapi.auth('exact-online', '', });
```

Add Connection configuration in Terapi by editing this page.
    
