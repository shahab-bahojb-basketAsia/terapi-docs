---
title: SmartRecruiters
sidebarTitle: SmartRecruiters
---

API configuration: [`smartrecruiters-api-key`](https://terapi.dev/providers.yaml)

## Features

| Features | Status |
| - | - |
| [Auth (Basic)](/integrate/guides/authorize-an-api) | ✅ |
| [Sync data](/integrate/guides/sync-data-from-an-api) | ✅ |
| [Perform workflows](/integrate/guides/perform-workflows-with-an-api) | ✅ |
| [Proxy requests](/integrate/guides/proxy-requests-to-an-api) | ✅ |
| [Receive webhooks](/integrate/guides/receive-webhooks-from-an-api) | 🚫 (time to contribute: &lt;48h) |

<Tip>We can implement missing features in &lt;48h, just ask for it in the [community](https://terapi.dev/slack).</Tip>

## Getting started

-   [Obtaining an API Key](https://developers.smartrecruiters.com/docs/authentication-api-key)
-   [SmartRecruiters API docs](https://developers.smartrecruiters.com/docs/the-smartrecruiters-platform)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

- SmartRecruiters uses API_KEY auth mode with X-SmartToken: `apiKey` in the request header to access different endpoints.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/smartrecruiters.mdx)</Note>