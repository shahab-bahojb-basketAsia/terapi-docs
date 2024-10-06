API configuration: [`twinfield`](https://terapi.dev/providers.yaml)

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

-   [Developer Portal](https://developers.twinfield.com/home)
-   [Api Reference](https://accounting.twinfield.com/webservices/documentation/#/)
-   [OpenID Connect Authentication](https://accounting.twinfield.com/webservices/documentation/#/ApiReference/Authentication/OpenIdConnect/#/)
-   [Scopes](https://accounting.twinfield.com/webservices/documentation/#/ApiReference/Authentication/OpenIdConnect#Scopes)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

-   During the OAuth flow, the user can decide to which resources (Bases) the app should have access to. [Read more here](https://airtable.com/developers/web/api/oauth-reference#resources)
-   Refresh tokens also expire after 60 days of non use. Make sure you call `terapi.getConnection()` at least every 60 days to trigger a refresh.

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/twinfield.mdx)