# Azure Web PubSub (microsoft-azure-web-pubsub)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Azure Web PubSub is a fully-managed service that enables building real-time, two-way messaging applications using publish-subscribe patterns over WebSockets. It supports broadcasting messages to clients in groups, sending messages to specific connections or users, and integrating with serverless event handlers for scalable real-time experiences.

**APIs.json:** [https://azure.microsoft.com/en-us/services/web-pubsub/](https://azure.microsoft.com/en-us/services/web-pubsub/)

## Tags

- Messaging
- Pub-Sub
- Real-Time
- Serverless
- WebSockets

## Timestamps

- **Created:** 2026-03-13
- **Modified:** 2026-05-30

## APIs

### Azure Web PubSub Service REST API

Data plane REST API for sending messages to connections, groups, and users on a Web PubSub service instance. Supports broadcast operations, targeted message delivery, and managing client lifecycle including disconnect operations and existence checks.

- **Human URL:** [https://learn.microsoft.com/en-us/rest/api/webpubsub/dataplane](https://learn.microsoft.com/en-us/rest/api/webpubsub/dataplane)
- **Base URL:** `https://{instance}.webpubsub.azure.com`

#### Tags

- Data Plane
- Messaging
- Web PubSub

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/webpubsub/dataplane)
- [OpenAPI](https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/webpubsub/data-plane/WebPubSub/stable/2024-01-01/webpubsub.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/dataplane/web-pub-sub)
- [Authentication](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/howto-generate-client-tokens)
- [Postman Collection](collections/microsoft-azure-web-pubsub.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-web-pubsub.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Azure Web PubSub Client and Upstream Events

AsyncAPI 2.6 description of the Azure Web PubSub client WebSocket subprotocols (json.webpubsub.azure.v1 and json.reliable.webpubsub.azure.v1) and the CloudEvents 1.0 HTTP upstream contract used by the service to deliver client events (connect, connected, disconnected, message, user custom events) to a configured backend webhook.

- **Human URL:** [https://learn.microsoft.com/en-us/azure/azure-web-pubsub/reference-json-webpubsub-subprotocol](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/reference-json-webpubsub-subprotocol)
- **Base URL:** `wss://{instance}.webpubsub.azure.com`

#### Tags

- AsyncAPI
- CloudEvents
- Event-Driven
- Pub-Sub
- WebSockets

#### Properties

- [AsyncAPI](https://raw.githubusercontent.com/api-evangelist/microsoft-azure-web-pubsub/main/asyncapi/microsoft-azure-web-pubsub-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Documentation](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/reference-json-webpubsub-subprotocol)
- [Reference](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/reference-json-reliable-webpubsub-subprotocol)
- [Reference](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/reference-cloud-events)
- [Authentication](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/howto-generate-client-tokens)
- [Postman Collection](collections/microsoft-azure-web-pubsub.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-web-pubsub.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Azure Web PubSub Management REST API

Control plane REST API for provisioning and managing Azure Web PubSub service instances. Supports creating, scaling, configuring, regenerating access keys, and deleting Web PubSub resources through Azure Resource Manager.

- **Human URL:** [https://learn.microsoft.com/en-us/rest/api/webpubsub](https://learn.microsoft.com/en-us/rest/api/webpubsub)
- **Base URL:** `https://management.azure.com`

#### Tags

- Control Plane
- Resource Manager
- Web PubSub

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/webpubsub)
- [OpenAPI](https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/webpubsub/resource-manager/Microsoft.SignalRService/stable/2024-03-01/webpubsub.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub)
- [Authentication](https://learn.microsoft.com/en-us/azure/active-directory/develop/authentication-scenarios)
- [Postman Collection](collections/microsoft-azure-web-pubsub.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-web-pubsub.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Azure Web PubSub Hubs REST API

REST API for managing hub configurations within a Web PubSub instance. Hubs provide logical isolation for messaging and allow per-hub configuration of event handlers, anonymous connect policies, and authorization settings.

- **Human URL:** [https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-hubs](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-hubs)
- **Base URL:** `https://management.azure.com`

#### Tags

- Hubs
- Resource Manager
- Web PubSub

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-hubs)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-hubs?view=rest-webpubsub-2024-03-01)
- [Postman Collection](collections/microsoft-azure-web-pubsub.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-web-pubsub.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Azure Web PubSub for Socket.IO REST API

REST API for managing Azure Web PubSub for Socket.IO instances. Provides a fully managed Socket.IO server replacement that allows existing Socket.IO applications to scale to millions of connections without rewriting application code.

- **Human URL:** [https://learn.microsoft.com/en-us/azure/azure-web-pubsub/socketio-overview](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/socketio-overview)
- **Base URL:** `https://management.azure.com`

#### Tags

- Resource Manager
- Socket.IO
- Web PubSub

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/socketio-overview)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub?view=rest-webpubsub-2024-03-01)
- [Getting Started](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/socketio-quickstart)
- [Postman Collection](collections/microsoft-azure-web-pubsub.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-web-pubsub.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Azure Web PubSub Private Endpoint Connections REST API

REST API for managing private endpoint connections to a Web PubSub service instance. Enables secure, private connectivity from virtual networks to Web PubSub through Azure Private Link without exposing traffic to the public internet.

- **Human URL:** [https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-private-endpoint-connections](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-private-endpoint-connections)
- **Base URL:** `https://management.azure.com`

#### Tags

- Networking
- Private Endpoints
- Resource Manager

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-private-endpoint-connections)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-private-endpoint-connections?view=rest-webpubsub-2024-03-01)
- [Postman Collection](collections/microsoft-azure-web-pubsub.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-web-pubsub.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Azure Web PubSub Shared Private Link Resources REST API

REST API for managing shared private link resources for a Web PubSub service. Enables outbound private connectivity from Web PubSub to other Azure resources such as Key Vault and Storage when configuring upstream event handlers.

- **Human URL:** [https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-shared-private-link-resources](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-shared-private-link-resources)
- **Base URL:** `https://management.azure.com`

#### Tags

- Networking
- Private Link
- Resource Manager

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-shared-private-link-resources)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-shared-private-link-resources?view=rest-webpubsub-2024-03-01)
- [Postman Collection](collections/microsoft-azure-web-pubsub.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/microsoft-azure-web-pubsub.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://portal.azure.com/)
- [Website](https://azure.microsoft.com/en-us/products/web-pubsub)
- [Documentation](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/)
- [Getting Started](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/quickstart-serverless)
- [Authentication](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/howto-generate-client-tokens)
- [Pricing](https://azure.microsoft.com/en-us/pricing/details/web-pubsub/)
- [S L A](https://azure.microsoft.com/en-us/support/legal/sla/web-pubsub/)
- [Status Page](https://status.azure.com/)
- [Blog](https://devblogs.microsoft.com/azure-sdk/)
- [Support](https://azure.microsoft.com/en-us/support/options/)
- [Terms of Service](https://azure.microsoft.com/en-us/support/legal/)
- [Privacy Policy](https://privacy.microsoft.com/en-us/privacystatement)
- [Sign Up](https://azure.microsoft.com/en-us/free)
- [Login](https://portal.azure.com)
- [S D Ks](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/reference-server-sdk-js)
- [S D K -  Java Script](https://www.npmjs.com/package/@azure/web-pubsub)
- [S D K -  Python](https://pypi.org/project/azure-messaging-webpubsubservice/)
- [S D K - . N E T](https://www.nuget.org/packages/Azure.Messaging.WebPubSub)
- [S D K -  Java](https://learn.microsoft.com/en-us/java/api/overview/azure/messaging-webpubsub-readme)
- [S D K -  Go](https://pkg.go.dev/github.com/Azure/azure-sdk-for-go/sdk/messaging/azwebpubsub)
- [C L I  Tools](https://learn.microsoft.com/en-us/cli/azure/webpubsub)
- [Changelog](https://azure.microsoft.com/en-us/updates/?product=web-pubsub)
- [GitHub Organization](https://github.com/Azure)
- [Git Hub  Samples](https://github.com/Azure/azure-webpubsub)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/azure-webpubsub)
- [Community](https://learn.microsoft.com/en-us/answers/tags/371/azure-web-pubsub)
- [F A Q](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/resource-faq)
- [Quotas](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/concept-billing-model)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
