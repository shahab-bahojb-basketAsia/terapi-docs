---
title: Payfit
sidebarTitle: Payfit
---

API configuration: [`payfit`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [How to register an Application](https://developers.payfit.io/docs/quickstart-guide#2%EF%B8%8F%E2%83%A3-become-a-payfit-partner)
-   [OAuth-related docs](https://developers.payfit.io/docs/implementing-the-oauth2-flow)
-   [List of OAuth scopes](https://developers.payfit.io/docs/scopes-2)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   Payfit does not return a refresh token, you will have to reauthorize the user again when it expires.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/payfit.mdx)</Note>
