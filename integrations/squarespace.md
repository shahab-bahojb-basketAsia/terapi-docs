API configuration: [`squarespace`](https://terapi.dev/providers.yaml)

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

-   [Request for developer OAuth credentials](https://partner.squarespace.com/oauth-form)
-   [OAuth-related docs](https://developers.squarespace.com/oauth)
-   [Squarespace REST API docs](https://developers.squarespace.com/commerce-apis/overview)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## API gotchas

-   Squarespace enforces different rate limits for different endpoints with a cool down period of one minute. For more details check [squarespace rate limits](https://developers.squarespace.com/commerce-apis/rate-limits)
-   Different APIs have different versions. Please confirm the latest version and append it to your resource endpoint, i.e `/{api-version}/commerce/inventory`
-   When creating a connection, you need to add the `customappDescription` configuration parameter, which will be appended to the request as a header: `User-Agent: YOUR_CUSTOM_APP_DESCRIPTION`. Requests without a valid `User-Agent` header are rejected.

Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/squarespace.mdx)