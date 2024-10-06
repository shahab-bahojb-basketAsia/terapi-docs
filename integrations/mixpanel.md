---
title: Mixpanel
sidebarTitle: Mixpanel
---

API configuration: [`mixpanel`](https://terapi.dev/providers.yaml)

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

-   [How to find API credentials (for end-users)](https://developer.mixpanel.com/reference/service-accounts)
-   [Auth docs](https://developer.mixpanel.com/reference/service-accounts)
-   [Web API docs (their REST API)](https://developer.mixpanel.com/reference/overview)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- For Basic auth, Mixpanel uses the service account username as username and service account secret as password.
- Mixpanel has [different API base URLs](https://docs.mixpanel.com/docs/other-bits/privacy-and-security/eu-residency) for querying data from European Unions projects.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/mixpanel.mdx)</Note>
