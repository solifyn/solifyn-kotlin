
# WebhookEntitlementGrantPayload

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) | The unique entitlement grant ID. |  [optional] |
| **businessId** | [**java.util.UUID**](java.util.UUID.md) | The business ID context. |  [optional] |
| **customerId** | [**java.util.UUID**](java.util.UUID.md) | The customer ID. |  [optional] |
| **paymentId** | [**java.util.UUID**](java.util.UUID.md) | Associated payment transaction ID. |  [optional] |
| **productId** | [**java.util.UUID**](java.util.UUID.md) | The purchased product ID. |  [optional] |
| **type** | **kotlin.String** | The type of entitlement (e.g. GITHUB). |  [optional] |
| **githubRepo** | **kotlin.String** | Target GitHub repository (owner/repo) if type is GITHUB. |  [optional] |
| **githubPermission** | **kotlin.String** | GitHub access permission level if type is GITHUB. |  [optional] |
| **githubUsername** | **kotlin.String** | The connected customer GitHub username. |  [optional] |
| **status** | **kotlin.String** | Delivery status of the collaborator invite (PENDING, DELIVERED, FAILED, REVOKED). |  [optional] |
| **oauthUrl** | **kotlin.String** | OAuth URL to redirect the customer to. |  [optional] |
| **errorDetails** | **kotlin.String** | Error message if invitation delivery failed. |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |



