---
title: NextCloud
sidebarTitle: NextCloud
---

API configuration: [`next-cloud-ocs`](https://terapi.dev/providers.yaml)

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

-   [NextCloud OCS basic auth related docs](https://docs.nextcloud.com/server/latest/developer_manual/client_apis/OCS/ocs-api-overview.html#authentication)
-   [NextCloud OCS API docs](https://docs.nextcloud.com/server/latest/developer_manual/client_apis/OCS/index.html)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- NextCloud OCS API uses `Basic` auth mode to access different endpoints. Provide your `username` as the Username value and `password` as the Password value. You will also need to provide the domain url when creating a connection.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/next-cloud.mdx)</Note>