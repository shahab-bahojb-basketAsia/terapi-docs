API configuration: [`stackexchange`](https://terapi.dev/providers.yaml)

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

-   [Register your OAuth app here](http://stackapps.com/apps/oauth/register)
-   [Stack Exchange API docs](https://api.stackexchange.com/docs)
-   [Stack Exchange OAuth scopes](https://api.stackexchange.com/docs/authentication#scope)
-   [Web API docs (their REST API)](https://api.stackexchange.com/docs)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

-   By default, access tokens expire (and cannot be refreshed). To get an access token that does not expire, pass the `no_expiry` scope (along with your other scopes).
-   Read the [usage notes here](https://api.stackexchange.com/docs/authentication#usage): You need to pass an additional `key` parameter together with your access token to benefit from higher API quotas.


    Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/stackexchange.mdx)