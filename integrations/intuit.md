---
title: Intuit
sidebarTitle: Intuit
---

API configuration: [`intuit`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).

## Getting started

-   [How to register an Application](https://developer.intuit.com/app/developer/qbo/docs/develop/authentication-and-authorization/oauth-2.0#create-an-app)
-   [OAuth-related docs](https://developer.intuit.com/app/developer/qbo/docs/develop/authentication-and-authorization/oauth-2.0)
-   [List of OAuth scopes](https://developer.intuit.com/app/developer/qbo/docs/learn/scopes)

Need help getting started? Get help in the [community](https://terapi.dev/slack).

## API gotchas

-   Refresh tokens have a rolling expiry of 100 days. If 100 days pass, or your refresh token expires, users need to go through the authorization flow again and reauthorize your app.

Add Getting Started links and Gotchas by [editing this page]()

