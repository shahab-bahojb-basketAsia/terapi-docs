---
title: Qualtrics
sidebarTitle: Qualtrics
---

API configuration: [`qualtrics`](https://terapi.dev/providers.yaml)

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

-   [Registering an App](https://developer.qualtrics.com/developer/portal/)
-   [OAuth-related docs](https://api.qualtrics.com/6c02f17c3109f-o-auth-authentication-auth-code)
-   [List of OAuth scopes](https://api.qualtrics.com/1450e85735dbf-o-auth-2-0-scopes)
-   [API reference](https://developer.qualtrics.com/developer/portal/documentation/1bd4e078a35c1-hello-world-setup)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## Connection configuration in terapi

Qualtrics requires a user specific subdomain to run OAuth.

You should request this from the user and pass it to terapi in the `terapi.auth()` call:

```js
terapi.auth('qualtrics', '<CONNECTION-ID>', {params: {subdomain: '<qualtrics-subdomain>'}});
```

For more details, see the [docs here](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).

## API gotchas

-   You are required to pass in the Data Center used to register your Qualtrics account as a subdomain for both the OAuth requests and subsequent API requests (cf. [Connection configuration](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization)).

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/qualtrics.mdx)</Note>
