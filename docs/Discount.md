
# Discount

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | The unique prefix-based identifier of the discount (e.g., &#x60;disc_cs8f67sd7f6fw3fs&#x60;). |  |
| **discountId** | **kotlin.String** | Alias for the unique identifier of the discount. |  |
| **code** | **kotlin.String** | The unique discount code (e.g. SAVE10) used during checkout. |  |
| **type** | [**inline**](#Type) | The discount calculation type: percentage or fixed_amount. |  |
| **amount** | **kotlin.Int** | The discount value. For percentage type, it is in basis points (e.g. 1000 &#x3D; 10.00%). For fixed_amount type, it is in cents (e.g. 1000 &#x3D; $10.00). |  |
| **usageLimit** | **kotlin.Int** | Maximum number of times this discount code can be redeemed. Null represents unlimited usage. |  |
| **timesUsed** | **kotlin.Int** | The number of times this discount code has been successfully redeemed. |  |
| **expiresAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | The expiration timestamp after which the discount code is no longer valid. |  |
| **status** | [**inline**](#Status) | The current status of the discount. |  |
| **businessId** | **kotlin.String** | The unique identifier associated with the business this discount belongs to. |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp indicating exactly when the discount was created. |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp indicating when the discount was last updated. |  |
| **name** | **kotlin.String** | The customer-facing name of the discount code (e.g. Summer Sale). |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | percentage, fixed_amount |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | active, expired |



