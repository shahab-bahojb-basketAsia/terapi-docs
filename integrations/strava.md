API configuration: [`strava`](https://terapi.dev/providers.yaml) for Mobile OAuth flow and [`strava-web`](https://terapi.dev/providers.yaml) for Web OAuth flow.

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

-   [How to register an Application](https://developers.strava.com/docs/getting-started/#account)
-   [OAuth-related docs](https://developers.strava.com/docs/authentication)
-   [List of OAuth scopes](https://developers.strava.com/docs/authentication/#details-about-requesting-access)
-   [Scopes Update](https://developers.strava.com/docs/oauth-updates/)
-   [Web API docs (their REST API)](https://developers.strava.com/playground)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

-   When adding the callback URL to Strava, you only have to add the domain of the URL and not the complete URL path.

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/strava.mdx)