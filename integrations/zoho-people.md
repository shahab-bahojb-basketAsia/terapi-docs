---
title: Zoho People
sidebarTitle: Zoho People
---

API configuration: [`zoho-people`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://www.zoho.com/people/api/oauth-steps.html#step1)
-   [OAuth-related docs](https://www.zoho.com/people/api/oauth-steps.html)
-   [List of OAuth scopes](https://www.zoho.com/people/api/scopes.html)
-   [Web API docs (their REST API)](https://www.zoho.com/people/api/overview.html)
-   [API rate limiting](https://www.zoho.com/people/api/api-limits.html)

<Tip>Do you need help? Please check this link [community](https://terapi.dev/slack).</Tip>

## Connection configuration in Terapi

- Zoho People uses [different domain extensions](https://www.zoho.com/people/api/oauth-steps.html#step3) for different regions.

Make sure to provide the required domain extension in the Terapi `terapi.auth()` call:

```js
terapi.auth('zoho-people', '<CONNECTION-ID>', {params: {extension: 'com'}});
```

For further information, visit the [docs here](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).

## API gotchas
- You can make your OAuth app cross-data-centers with [these instructions](https://www.zoho.com/accounts/protocol/oauth/multi-dc.html#:~:text=Steps%20to%20enable%20Multi%20DC%20support&text=Go%20to%20the%20Settings%20tab,have%20a%20unique%20client%20secret). This allows a single OAuth app to query the Zoho People API across different data centers, such as those in the US, EU, and other regions.

<Note>
    Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/zoho-people.mdx)
</Note>
