---
title: Intercom
sidebarTitle: Intercom
---

API configuration: [`intercom`](https://terapi.dev/providers.yaml)

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

-   [Create a Developer Workspace](https://app.intercom.com/a/developer-signup)
-   [How to register an Application](https://developers.intercom.com/building-apps/docs/setting-up-oauth)
-   [OAuth-related docs](https://developers.intercom.com/building-apps/docs/setting-up-oauth)
-   [List of OAuth scopes](https://developers.intercom.com/building-apps/docs/oauth-scopes)
-   [Web API docs (their REST API)](https://developers.intercom.com/building-apps/docs/rest-apis)

Need help getting started? Get help in the [community](https://terapi.dev/slack).

## API gotchas

-   Intercom access tokens do not expire. Logically, Intercom doesn't return a refresh token along with the access token.
-   You do not need to pass API scopes/permissions during the authorization request. Permissions are only set in the Intercom Developer Portal.

Add Getting Started links and Gotchas by [editing this page]()

