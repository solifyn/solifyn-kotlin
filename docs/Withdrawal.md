
# Withdrawal

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | The local withdrawal ID |  |
| **whopId** | **kotlin.String** | The Whop withdrawal ID |  |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The amount withdrawn in cents |  |
| **currency** | **kotlin.String** | Three-letter ISO currency code |  |
| **status** | **kotlin.String** | The status of the withdrawal request |  |
| **businessId** | **kotlin.String** | The business ID associated with this withdrawal |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the withdrawal was requested |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the withdrawal status was updated |  |
| **feeAmount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Fee amount charged for the withdrawal in cents |  [optional] |
| **feeType** | **kotlin.String** | The fee structure type (inclusive or exclusive) |  [optional] |
| **markupFee** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Markup fee applied in cents |  [optional] |
| **speed** | **kotlin.String** | Speed of withdrawal (standard, instant) |  [optional] |
| **traceCode** | **kotlin.String** | Bank trace or reference code for tracking the payout |  [optional] |
| **payerName** | **kotlin.String** | The name of the entity or account paying out |  [optional] |
| **errorMessage** | **kotlin.String** | Error message if the withdrawal failed |  [optional] |



