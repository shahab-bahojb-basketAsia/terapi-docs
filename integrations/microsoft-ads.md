---
title: Microsoft Ads
sidebarTitle: Microsoft Ads
---

API configuration: [`microsoft-ads`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (OAuth)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | 🚫 (see API gotchas) |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | 🚫 (see API gotchas) |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | 🚫 (see API gotchas) |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [Microsoft Ads Authentication with OAuth](https://learn.microsoft.com/en-us/advertising/guides/authentication-oauth?view=bingads-13)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   The Microsoft Advertising API doesn't offer a REST API, which means certain terapi functionalities won't be accessible, including syncs, workflows, and proxy requests.  
    To engage with the Microsoft Advertising API, developers must initially retrieve the access token utilizing the [backend API](https://docs.terapi.dev/reference/api/connection/get). This token should then be utilized with [official client libraries](https://learn.microsoft.com/en-us/advertising/guides/client-libraries?view=bingads-13) or a [SOAP Client](https://learn.microsoft.com/en-us/advertising/guides/authentication-oauth-quick-start?view=bingads-13) for further interaction.

<Note>
    Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/microsoft-ads.mdx)
</Note>

