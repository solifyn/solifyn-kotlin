
# EntitlementGrantResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) | The unique entitlement grant ID. |  |
| **businessId** | [**java.util.UUID**](java.util.UUID.md) | The business ID context. |  |
| **customerId** | [**java.util.UUID**](java.util.UUID.md) | The customer ID. |  |
| **productId** | [**java.util.UUID**](java.util.UUID.md) | The purchased product ID. |  |
| **type** | **kotlin.String** | The type of entitlement (e.g. GITHUB, DISCORD, TELEGRAM). |  |
| **status** | **kotlin.String** | Delivery status of the collaborator invite (PENDING, DELIVERED, FAILED, REVOKED). |  |
| **createdAt** | **kotlin.String** | Creation timestamp. |  |
| **updatedAt** | **kotlin.String** | Modification timestamp. |  |
| **paymentId** | [**java.util.UUID**](java.util.UUID.md) | Associated payment transaction ID. |  [optional] |
| **githubRepo** | **kotlin.String** | Target GitHub repository (owner/repo) if type is GITHUB. |  [optional] |
| **githubPermission** | **kotlin.String** | GitHub access permission level if type is GITHUB. |  [optional] |
| **githubUsername** | **kotlin.String** | The connected customer GitHub username. |  [optional] |
| **discordGuildId** | **kotlin.String** | Target Discord Guild ID if type is DISCORD. |  [optional] |
| **discordRoleId** | **kotlin.String** | Target Discord Role ID if type is DISCORD. |  [optional] |
| **discordUsername** | **kotlin.String** | The connected customer Discord username. |  [optional] |
| **discordUserId** | **kotlin.String** | The connected customer Discord user ID. |  [optional] |
| **oauthUrl** | **kotlin.String** | OAuth URL to redirect the customer to. |  [optional] |
| **errorDetails** | **kotlin.String** | Error message if invitation delivery failed. |  [optional] |
| **metadata** | [**kotlin.Any**](.md) | Platform-specific metadata. |  [optional] |



