
# SubscriptionAction

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **freeDays** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Number of free days to add (used with action: add_free_days) |  [optional] |
| **cancellationMode** | [**inline**](#CancellationMode) | Cancellation mode (used with action: cancel) |  [optional] |
| **voidPayments** | **kotlin.Boolean** | Whether to void subsequent payments (used with action: pause) |  [optional] |
| **addonProductId** | **kotlin.String** | ID of the addon product to adjust seats for (used with action: adjust_seats) |  [optional] |
| **newQuantity** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The new seat quantity (used with action: adjust_seats) |  [optional] |
| **prorationType** | [**inline**](#ProrationType) | Proration strategy mode (used with action: adjust_seats) |  [optional] |
| **idempotencyKey** | **kotlin.String** | A unique idempotency key to prevent duplicate mutative actions for network transient retries. |  [optional] |


<a id="CancellationMode"></a>
## Enum: cancellation_mode
| Name | Value |
| ---- | ----- |
| cancellationMode | immediate, at_period_end |


<a id="ProrationType"></a>
## Enum: prorationType
| Name | Value |
| ---- | ----- |
| prorationType | prorated_immediately, full_immediately, difference_immediately, do_not_bill |



