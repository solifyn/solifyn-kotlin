
# DiscountCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **code** | **kotlin.String** | Unique discount code string (will be automatically capitalized). |  |
| **type** | [**inline**](#Type) | Calculation type: percentage or fixed_amount. |  |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The discount value. If percentage, enter value like 10 for 10%. If fixed_amount, enter value like 10 for $10.00. |  |
| **name** | **kotlin.String** | Customer-facing name of the discount. |  [optional] |
| **usageLimit** | **kotlin.Int** | Maximum number of redemptions allowed. |  [optional] |
| **expiresAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Expiration timestamp for the discount. |  [optional] |
| **subscriptionCycles** | **kotlin.Int** | Number of subscription cycles this discount applies to. |  [optional] |
| **restrictedTo** | **kotlin.collections.List&lt;kotlin.String&gt;** | List of product IDs this discount is restricted to. |  [optional] |
| **preserveOnPlanChange** | **kotlin.Boolean** | Whether to preserve the discount when subscription plan changes. |  [optional] |
| **metadata** | [**kotlin.Any**](.md) | Custom metadata for the discount. |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | percentage, fixed_amount |



