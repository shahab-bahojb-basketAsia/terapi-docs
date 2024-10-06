---
title: Pivotaltracker
sidebarTitle: Pivotaltracker
---

API configuration: [`pivotaltracker`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (Basic)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [Generate an API token in your Pivotaltracker account](https://www.pivotaltracker.com/profile)
-   [Pivotaltracker API docs](https://www.pivotaltracker.com/help/api)
-   [Authentication and API token](https://www.pivotaltracker.com/help/api#Basics)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- Pivotaltracker uses `API_KEY` auth mode with `X-TrackerToken: api_key` as a request header to access different endpoints.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/pivotaltracker.mdx)</Note>