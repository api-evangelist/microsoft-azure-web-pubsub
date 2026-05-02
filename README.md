# Azure Web PubSub (microsoft-azure-web-pubsub)
Azure Web PubSub is a fully-managed service that enables building real-time, two-way messaging applications using publish-subscribe patterns over WebSockets. It supports broadcasting messages to clients in groups, sending messages to specific connections or users, and integrating with serverless event handlers for scalable real-time experiences.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/microsoft-azure-web-pubsub/refs/heads/main/apis.yml)

## Tags:

 - Messaging, Pub-Sub, Real-Time, Serverless, WebSockets

## Timestamps

- **Created:** 2026-03-13
- **Modified:** 2026-04-28

## APIs

### Azure Web PubSub Service REST API
Data plane REST API for sending messages to connections, groups, and users on a Web PubSub service instance. Supports broadcast operations, targeted message delivery, and managing client lifecycle including disconnect operations and existence checks.

**Human URL:** [https://learn.microsoft.com/en-us/rest/api/webpubsub/dataplane](https://learn.microsoft.com/en-us/rest/api/webpubsub/dataplane)

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/webpubsub/dataplane)
- [OpenAPI](https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/webpubsub/data-plane/WebPubSub/stable/2024-01-01/webpubsub.json)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/dataplane/web-pub-sub)
- [Authentication](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/howto-generate-client-tokens)

### Azure Web PubSub Management REST API
Control plane REST API for provisioning and managing Azure Web PubSub service instances. Supports creating, scaling, configuring, regenerating access keys, and deleting Web PubSub resources through Azure Resource Manager.

**Human URL:** [https://learn.microsoft.com/en-us/rest/api/webpubsub](https://learn.microsoft.com/en-us/rest/api/webpubsub)

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/webpubsub)
- [OpenAPI](https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/webpubsub/resource-manager/Microsoft.SignalRService/stable/2024-03-01/webpubsub.json)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub)
- [Authentication](https://learn.microsoft.com/en-us/azure/active-directory/develop/authentication-scenarios)

### Azure Web PubSub Hubs REST API
REST API for managing hub configurations within a Web PubSub instance. Hubs provide logical isolation for messaging and allow per-hub configuration of event handlers, anonymous connect policies, and authorization settings.

**Human URL:** [https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-hubs](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-hubs)

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-hubs)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-hubs?view=rest-webpubsub-2024-03-01)

### Azure Web PubSub for Socket.IO REST API
REST API for managing Azure Web PubSub for Socket.IO instances. Provides a fully managed Socket.IO server replacement that allows existing Socket.IO applications to scale to millions of connections without rewriting application code.

**Human URL:** [https://learn.microsoft.com/en-us/azure/azure-web-pubsub/socketio-overview](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/socketio-overview)

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/socketio-overview)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub?view=rest-webpubsub-2024-03-01)
- [Getting Started](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/socketio-quickstart)

### Azure Web PubSub Private Endpoint Connections REST API
REST API for managing private endpoint connections to a Web PubSub service instance. Enables secure, private connectivity from virtual networks to Web PubSub through Azure Private Link without exposing traffic to the public internet.

**Human URL:** [https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-private-endpoint-connections](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-private-endpoint-connections)

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-private-endpoint-connections)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-private-endpoint-connections?view=rest-webpubsub-2024-03-01)

### Azure Web PubSub Shared Private Link Resources REST API
REST API for managing shared private link resources for a Web PubSub service. Enables outbound private connectivity from Web PubSub to other Azure resources such as Key Vault and Storage when configuring upstream event handlers.

**Human URL:** [https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-shared-private-link-resources](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-shared-private-link-resources)

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-shared-private-link-resources)
- [Reference](https://learn.microsoft.com/en-us/rest/api/webpubsub/web-pub-sub-shared-private-link-resources?view=rest-webpubsub-2024-03-01)

## Common Properties

- [Portal](https://portal.azure.com/)
- [Website](https://azure.microsoft.com/en-us/products/web-pubsub)
- [Documentation](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/)
- [Getting Started](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/quickstart-serverless)
- [Authentication](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/howto-generate-client-tokens)
- [Pricing](https://azure.microsoft.com/en-us/pricing/details/web-pubsub/)
- [SLA](https://azure.microsoft.com/en-us/support/legal/sla/web-pubsub/)
- [Status](https://status.azure.com/)
- [Support](https://azure.microsoft.com/en-us/support/options/)
- [Terms of Service](https://azure.microsoft.com/en-us/support/legal/)
- [Privacy Policy](https://privacy.microsoft.com/en-us/privacystatement)
- [Sign Up](https://azure.microsoft.com/en-us/free)
- [SDK - JavaScript](https://www.npmjs.com/package/@azure/web-pubsub)
- [SDK - Python](https://pypi.org/project/azure-messaging-webpubsubservice/)
- [SDK - .NET](https://www.nuget.org/packages/Azure.Messaging.WebPubSub)
- [SDK - Java](https://learn.microsoft.com/en-us/java/api/overview/azure/messaging-webpubsub-readme)
- [SDK - Go](https://pkg.go.dev/github.com/Azure/azure-sdk-for-go/sdk/messaging/azwebpubsub)
- [CLI Tools](https://learn.microsoft.com/en-us/cli/azure/webpubsub)
- [GitHub Samples](https://github.com/Azure/azure-webpubsub)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/azure-webpubsub)
- [FAQ](https://learn.microsoft.com/en-us/azure/azure-web-pubsub/resource-faq)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
