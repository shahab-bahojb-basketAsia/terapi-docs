---
title: Notion
sidebarTitle: Notion
---

API configuration: [`notion`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://developers.notion.com/docs/authorization)
-   [OAuth-related docs](https://developers.notion.com/docs/authorization#public-integration-auth-flow-set-up)
-   [API reference](https://developers.notion.com/reference/intro)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- The Notion OAuth API doesn't support refreshing tokens, and so doesn't return a refresh token. The access token never expires.
- Your Notion OAuth app will have the status "internal". You need to [make it "public"](https://developers.notion.com/docs/authorization#how-to-make-an-integration-public) to be able to initiate an OAuth flow. Only then, you will be able to get the OAuth client ID/secret and register your callback URL.
- No OAuth scope is required by default.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/notion.mdx)</Note>
