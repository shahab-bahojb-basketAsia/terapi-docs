---
title: Monday
sidebarTitle: Monday
---

API configuration: [`monday`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://developer.monday.com/apps/docs/oauth#registering-a-monday-app)
-   [OAuth-related docs](https://developer.monday.com/apps/docs/oauth)
-   [List of OAuth scopes](https://developer.monday.com/apps/docs/oauth#set-up-permission-scopes)
-   [API](https://developer.monday.com/apps/docs/quickstart-integration)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   Access tokens do not expire and will be valid until the user uninstalls your app. Our OAuth flow does not support refresh tokens at the moment.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/monday.mdx)</Note>
