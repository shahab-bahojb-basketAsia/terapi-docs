---
title: Metabase
sidebarTitle: Metabase
---

API configuration: [`metabase`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (API Key)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [How to generate a Metabase API key](https://www.metabase.com/docs/latest/people-and-groups/api-keys#create-an-api-key)
-   [Metabase Authentication](https://www.metabase.com/docs/latest/people-and-groups/api-keys#example-get-requests)
-   [Metabase API docs](https://www.metabase.com/docs/latest/api-documentation)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- Metabase uses API_KEY authentication mode with `x-api-key: API_KEY` as a request header to access different endpoints.
- When creating a new connection on terapi, you will have to provide your domain. If your Metabase is at `https://your-metabase.com` you could access the APIs at `https://your-metabase.com/api/database`.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/metabase.mdx)</Note>