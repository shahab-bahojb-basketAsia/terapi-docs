---
title: Personio
sidebarTitle: Personio
---

API configurations: [`personio`](https://terapi.dev/providers.yaml), [`personio-recruiting`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://developer.personio.de/docs/getting-started-with-the-personio-api)
-   [OAuth-related docs](https://developer.personio.de/reference/auth)
-   [Web API docs (their REST API)](https://developer.personio.de/reference/introduction)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   Personio offers a separate recruiting API that is API key based and is listed under `personio-recruiting`
-   The other API Personio offers is a client credentials token that authorizes as app instead of a user. This is listed under `personio`.
-   The `companyId` value is required for `personio-recruiting` and can be retrieved at Settings > Integrations (API Credentials) and clicking on the "Recruiting API Key".
    The value for `company` as required for `personio-recruiting` is the name you use to login to your account
    and is the subdomain of your Personio instance.
-   The values for `partnerId` and `appId` are optional but strongly recommended by Personio. Both can be defined by you, but should represent your company name and application name and MUST follow the UPPER_SNAKE_CASE format. For example `MY_APPLICATION`, `ACME` are valid values.
    An example of setting them in the `terapi.auth` call:
    ```ts
    terapi.auth('personio-recruiting', 'test-connection-id', { params: { companyId: '33434', partnerId: 'YOUR_CUSTOM_NAME', appId: 'UNIQUE_ID', company: 'company-b' },
        credentials: {
          apiKey: '<secure-key>'
        }
      })
      .then((result: { providerConfigKey: string; connectionId: string }) => {
        // do something
      }).catch((err: { message: string; type: string }) => {
        // handle error
      });

    terapi.auth('personio', 'test-connection-id', { params: { partnerId: 'YOUR_CUSTOM_NAME', appId: 'UNIQUE_NAME' },
        credentials: {
            client_id: '<your-client-id>',
            client_secret: '<your-client-secret>'
        }
      })
      .then((result: { providerConfigKey: string; connectionId: string }) => {
        // do something
      }).catch((err: { message: string; type: string }) => {
        // handle error
      });
    ```


<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/personio.mdx)</Note>
