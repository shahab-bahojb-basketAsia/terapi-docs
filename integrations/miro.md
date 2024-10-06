---
title: Miro
sidebarTitle: Miro
---

API configuration: [`miro`](https://terapi.dev/providers.yaml)

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

-   [Registering an App](https://developers.miro.com/docs/rest-api-build-your-first-hello-world-app#step-1-create-your-app-in-miro)
-   [OAuth-related docs](https://developers.miro.com/docs/getting-started-with-oauth)
-   [List of OAuth scopes](https://developers.miro.com/reference/scopes)
-   [API reference](https://developers.miro.com/reference/api-reference)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   An access token expires in an hour and a refresh token expires in 60 days.
-   You can use the `terapi.getConnection('<CONFIG-KEY>', '<CONNECTION-ID>')` to refresh the token, and the token will be refreshed if it is expired.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/miro.mdx)</Note>
