API configuration: [`wildix-pbx`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).

## Getting started

-   [How to register an Application](https://wildix.atlassian.net/wiki/x/3B-OAQ)
-   [Api documentation for Wildix PBX](https://docs.wildix.com/wms/index.html)
-   [OAuth-related docs](https://docs.wildix.com/wms/index.html#section/Authentication)
-   [List of OAuth scopes](https://docs.wildix.com/wms/index.html#section/Authentication)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## Connection configuration in Terapi

Wildix PBX requires a PBX specific subdomain to run OAuth `demo-pbx`.wildixin.com

You should request this from the user and pass it to Terapi in the `terapi.auth()` call:

```js
terapi.auth('wildix-pbx', '', {params: {subdomain: ''}});
```

For more details, see the [docs here](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).

## API gotchas

_None yet, add yours!_

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/wildix.mdx)