---
title: Avalara
sidebarTitle: Avalara
---

API configuration: `avalara`, `avalara-sandbox`

## Features

| Features | Status |
| - | - |
| [Auth (Basic)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](https://terapi.gitbook.io/terapi-api-explorer/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

We can implement missing features in &lt;48h, just ask for it in the community.

## Getting started

-   [Avalara authentication](https://developer.avalara.com/avatax/authentication-in-rest)
-   [Avalara API docs](https://developer.avalara.com/api-reference/avatax/rest/v2/)

Do you need help? Please check this link.

## API gotchas

- Avalara uses BASIC authentication to access various AvaTax API endpoints. You can provide either a combination of your `username` and `password` or your `accountID` and `licensekey` to authenticate with the Avalara AvaTax API. The license key can be generated by an account administrator under Settings > Reset License Key.
- When creating a new connection on Terapi, please provide the `avalaraClient`, which can help you diagnose and resolve issues with your software when used appropriately. This value is a combination of `(app name); (app version); (library name); (library version); (machine name)`. For more details, refer to [Client Headers](https://developer.avalara.com/avatax/client-headers/)

Add Getting Started links and Gotchas by editing this page.

