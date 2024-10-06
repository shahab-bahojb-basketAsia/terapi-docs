---
title: Ory
sidebarTitle: Ory
---

API configurations: [`ory`](https://terapi.dev/providers.yaml)

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

-   [OAuth related docs](https://www.ory.sh/docs/oauth2-oidc/client-credentials#body-authentication)
-   [Ory REST API docs](https://www.ory.sh/docs/welcome)
-   [List of Oauth scopes](https://www.ory.sh/docs/oauth2-oidc/openid-connect-claims-scope-custom)

<Tip>Need help getting started? Get help in the [community](https://terapi.dev/slack).</Tip>

## API gotchas

-   When creating a new application, you need to supply your `project_id`. This can be located under the Project Settings tab for the specific project.
-   When creating a new connection in terapi, you will need to add your `projectSlug`, which is also located under the Project Settings tab for the specific project.
<Note>Add Getting Started links and Gotchas by [editing this page](https://github.com/terapihq/terapi/tree/master/docs-v2/integrations/all/ory.mdx)</Note>
