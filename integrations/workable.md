API configuration: [`workable`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (API Key)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).

## Getting started

Workable offers API keys ("API access token"), partner tokens, and OAuth for authentication. Terapi currently only supports API-key-based authentication.

-   [API Docs](https://workable.readme.io/reference)
-   [How to generate an API key](https://workable.readme.io/reference/generate-an-access-token#generate-an-api-access-token)
-   [Workable API rate limits](https://workable.readme.io/reference/rate-limits)
-   [Web API docs (their REST API)](https://workable.readme.io/reference/accounts)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## Connection configuration in Terapi

Workable requires a user specific subdomain for the API base URL.

You should request this from the user and pass it to Terapi in the `terapi.auth()` call:

```js
terapi.auth('workable', '', {params: {subdomain: ''}});
```

For more details see the [docs here](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).

## API gotchas

- To authorize a Workable Connection in Terapi you need to pass both the API key and the company's workable subdomain:
```js
terapi.auth('workable', '', {
        credentials: {
            apiKey: ''
        },
        params: {
            subdomain: ''
        }});
```

- The API base URL in Terapi is set to `https://{subdomain}.workable.com` for future forward compatability. To call endpoints of the V3 API, prefix the endpoint with `/spi/v3/`, e.g. `/spi/v3/candidates`.

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/workable.mdx)