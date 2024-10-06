---
title: Quickbooks
sidebarTitle: Quickbooks
---

API configuration: [`quickbooks`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://developer.intuit.com/app/developer/qbo/docs/develop/authentication-and-authorization/oauth-2.0#create-an-app)
-   [OAuth-related docs](https://developer.intuit.com/app/developer/qbo/docs/develop/authentication-and-authorization)
-   [List of OAuth scopes](https://developer.intuit.com/app/developer/qbo/docs/learn/scopes#current-scopes)
-   [Quickbooks API docs](https://developer.intuit.com/app/developer/qbo/docs/api/accounting/all-entities/account)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- Quickbooks requires a company ID for each API request. Quickbooks returns it as part of the OAuth flow, and terapi stores it automatically in the `connection_config` for you with the key `realmId`.
    - You can use [getConnection](/reference/scripts#get-the-connection-credentials) in your integration scripts to retrieve it, or when you fetch the Connection credentials with the REST API or SDK

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/quickbooks.mdx)</Note>
