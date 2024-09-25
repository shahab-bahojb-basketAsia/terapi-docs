---
title: Amazon
sidebarTitle: Amazon
---

API configuration: `amazon`

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

-   [How to register an Application](https://developer.amazon.com/docs/login-with-amazon/register-web.html)
-   [OAuth-related docs](https://developer.amazon.com/docs/login-with-amazon/authorization-code-grant.html)
-   [List of OAuth scopes](https://developer.amazon.com/docs/login-with-amazon/customer-profile.html)

Do you need help? Please check this link.

## Connection configuration in Terapi

Amazon uses different domain extensions for various regions. For example, `amazon.com` for the US, `amazon.co.uk` for the UK, or `amazon.de` for Germany.

You should provide the domain extension to Terapi in the `terapi.auth()` call:

```js
terapi.auth('amazon', '', });

