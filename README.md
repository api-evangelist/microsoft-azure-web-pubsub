# Azure Web PubSub (microsoft-azure-web-pubsub)

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
