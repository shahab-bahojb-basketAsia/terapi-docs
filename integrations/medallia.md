---
title: Medallia
sidebarTitle: Medallia
---

API configurations: [`medallia`](https://terapi.dev/providers.yaml)

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

-   [How to build an app](https://developer.medallia.com/medallia-apps/docs/register-as-an-app-builder)
-   [OAuth related docs](https://developer.medallia.com/medallia-apis/reference/authentication)
-   [Medallia REST API docs](https://developer.medallia.com/medallia-apis/reference/integrations)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas
-   Medallia enforces different rate limits based on the API types. For more details check [Medallia rate and limits](https://developer.medallia.com/medallia-apis/reference/integrations#rates-and-limits).
-   When creating a new connection, you will need to supply your `reportingInstance` and `tenantName`. The `instance` and `tenant` values are taken from the Reporting URL, such as `instance.medallia.com/tenant`.
-   You will also need to provide your `gatewayUrl` so as to build your terapi proxy `base_url`. This is in the form of `instance-tenant.apis.medallia.com`. The suffix `apis.medallia.com` is constant, independent of the data center. The Reporting URL is set when your Experience Cloud instance is first provisioned. For more details on this check [production instance and partner sandboxes](https://developer.medallia.com/medallia-apis/reference/integrations#production-instances-and-partner-sandboxes)
<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/medallia.mdx)</Note>
