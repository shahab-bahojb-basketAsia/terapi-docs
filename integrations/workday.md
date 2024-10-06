API configuration: [`workday`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (API Key)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | 🚫 |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).

## Getting started

Workday provides two APIs, a REST and a SOAP one. Only the SOAP is currently supported.

## Connection configuration in Terapi

Workday requires a user specific subdomain for the API base URL.

You should request this from the user and pass it to Terapi in the `terapi.auth()` call:

```js
terapi.auth('workday', '', {params: {subdomain: ''}});
```

For more details see the [docs here](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).

## API gotchas

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/workday.mdx)