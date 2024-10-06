---
title: Zoho Bigin
sidebarTitle: Zoho Bigin
---

API configuration: [`zoho-bigin`](https://terapi.dev/providers.yaml)

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

-   [Register an Application](https://accounts.zoho.com/developerconsole)
-   [OAuth-related docs](https://www.bigin.com/developer/docs/apis/v2/oauth-overview.html)
-   [List of OAuth scopes](https://www.bigin.com/developer/docs/apis/v2/scopes.html)
-   [Web API docs (their REST API)](https://www.bigin.com/developer/docs/apis/v2/)

<Tip>Do you need help? Please check this link [community](https://terapi.dev/slack).</Tip>

## Connection configuration in Terapi

Zoho uses [different domain extensions](https://www.bigin.com/developer/docs/apis/multi-dc.html) for different regions.

Make sure to provide the required domain extension in the Terapi `terapi.auth()` call:

```js
terapi.auth('zoho-bigin', '<CONNECTION-ID>', {params: {extension: 'com'}});
```

For further information, visit the [docs here](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).

## API gotchas
- You can make your OAuth app cross-data-centers with [these instructions](https://www.bigin.com/developer/docs/apis/multi-dc.html). This allows a single OAuth application to make requests to the Zoho API for Zoho accounts from the US, EU, etc.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/zoho-bigin.mdx)</Note>
