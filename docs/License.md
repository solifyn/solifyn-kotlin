
# License

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | The unique prefix-based identifier of the license key. |  |
| **key** | **kotlin.String** | The cryptographically generated license key string delivered to the customer. |  |
| **status** | [**inline**](#Status) | Lifecycle status of the license. ACTIVE &#x3D; active. DISABLED &#x3D; suspended. REVOKED &#x3D; hard-revoked. |  |
| **businessId** | **kotlin.String** | The unique identifier associated with the business this license belongs to. |  |
| **productId** | **kotlin.String** | The unique ID of the product this license key is associated with. |  |
| **paymentId** | **kotlin.String** | The unique payment identifier that triggered the issuance of this license key. |  |
| **customerId** | **kotlin.String** | The unique customer identifier (ID) who received this license key. |  |
| **activationLimit** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Maximum number of simultaneous active device instances allowed for this license. Null means unlimited. |  |
| **activationMessage** | **kotlin.String** | Optional message displayed to the customer upon successful activation. |  |
| **instancesCount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Running count of how many times this license key has been activated. |  |
| **expiryHours** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Relative expiry duration in hours from the time of issuance. |  |
| **expiresAt** | **kotlin.String** | Absolute expiration timestamp. The license becomes invalid after this point. |  |
| **filters** | [**kotlin.Any**](.md) | Optional custom metadata filters associated with the license. |  |
| **archived** | **kotlin.Boolean** | Indicates if the license key is archived. |  |
| **createdAt** | **kotlin.String** | Timestamp indicating exactly when the license key was issued. |  |
| **updatedAt** | **kotlin.String** | Timestamp indicating when the license key was last modified. |  |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | ACTIVE, DISABLED, REVOKED |



