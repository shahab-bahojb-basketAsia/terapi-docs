API configuration: [`zoho-invoice`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://accounts.zoho.com/developerconsole)
-   [OAuth-related docs](https://www.zoho.com/invoice/api/v3/oauth/#overview)
-   [List of OAuth scopes](https://www.zoho.com/invoice/api/v3/oauth/#overview:~:text=List%20of%20scopes%20available%20in%20Zoho%20Invoice%20%3A)
-   [Web API docs (their REST API)](https://www.zoho.com/invoice/api/v3/apicollection/#overview)

Do you need help? Please check this link [community](https://terapi.dev/slack).

## Connection configuration in Terapi

Zoho uses [different domain extensions](https://www.zoho.com/crm/developer/docs/api/v3/multi-dc.html) for different regions. 

You need to pass the domain extension to use to Terapi in the `terapi.auth()` call:

```js
terapi.auth('zoho-invoice', '', {params: {extension: 'com'}});
```

For more details, see the [docs here](/integrate/guides/authorize-an-api#apis-requiring-connection-specific-configuration-for-authorization).

## API gotchas
- You can make your OAuth app cross-data-centers with [these instructions](https://www.zoho.com/crm/developer/docs/api/v3/multi-dc.html). This means that a single OAuth app will be able to query the Zoho API for Zoho accounts from the US, EU, etc.


    Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/zoho-invoice.mdx)