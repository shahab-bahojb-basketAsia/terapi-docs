---
title: Mailchimp
sidebarTitle: Mailchimp
---

API configuration: [`mailchimp`](https://terapi.dev/providers.yaml)

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

-   [OAuth-related docs](https://mailchimp.com/developer/marketing/guides/access-user-data-oauth-2)
-   [How Register an Application](https://mailchimp.com/developer/marketing/guides/access-user-data-oauth-2/#register-your-application)
-   [Web API docs (their REST api)](https://mailchimp.com/developer/marketing/api/root/)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   Mailchimp do not use scopes during Authorization. Hence, when providing scopes in the provider configuration in the terapi UI, you can ignore.

<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/mailchimp.mdx)</Note>