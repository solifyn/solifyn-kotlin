
# SubscriptionSeatAdjustment

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **success** | **kotlin.Boolean** | Indicates if the seat adjustment was successful |  |
| **subscriptionId** | **kotlin.String** | The customer subscription ID |  |
| **addonProductId** | **kotlin.String** | The unique ID of the addon product |  |
| **oldQuantity** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The previous seat quantity |  |
| **newQuantity** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The new seat quantity after adjustment |  |
| **quantityDelta** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The difference in seat quantity |  |
| **prorationType** | **kotlin.String** | The proration strategy type applied |  |
| **costImpact** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Calculated pro-rata price cost impact in currency unit (charged or credited) |  |
| **currency** | **kotlin.String** | Billing currency |  |



