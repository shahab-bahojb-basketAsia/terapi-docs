---
title: Microsoft Power Bi
sidebarTitle: Microsoft Power Bi
---

API configuration: [`microsoft-power-bi`](https://terapi.dev/providers.yaml)

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

-   [How to register an Application](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app)
-   [OAuth related docs](https://learn.microsoft.com/en-us/power-bi/developer/embedded/embed-tokens?tabs=embed-for-customers)
-   [Microsoft Power Bi REST API docs](https://learn.microsoft.com/en-us/rest/api/power-bi/)


<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   You can find scopes required for each API call in their corresponding API calls section. For example, to retrieve a list of datasets from My workspace, you can refer to the Required scope section of the [Get Datasets](https://learn.microsoft.com/en-us/rest/api/power-bi/datasets/get-datasets#required-scope) documentation. You also need to prepend the hostname to the scope, which in the get datasets example would be `https://analysis.windows.net/powerbi/api/Dataset.ReadWrite.All`. For more details, check [this resource out](https://community.fabric.microsoft.com/t5/Service/Azure-AD-App-Authentication-scope-doesn-t-exist-on-app-with/m-p/3074525/highlight/true#M188140).
-   Please be aware that the Microsoft Power Bi implements throttling to manage the volume of requests. For more information on handling throttling, refer to the [Microsoft Power Bi Throttling Guidance](https://learn.microsoft.com/en-us/rest/api/power-bi/#throttling).

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/microsoft-power-bi.mdx)</Note>
