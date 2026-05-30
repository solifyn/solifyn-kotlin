
# Refund

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) | The refund ID |  |
| **whopId** | **kotlin.String** | The Whop Refund ID |  |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Refunded amount |  |
| **currency** | **kotlin.String** | Currency code |  |
| **status** | [**inline**](#Status) | Status of the refund |  |
| **paymentId** | [**java.util.UUID**](java.util.UUID.md) | The associated Payment ID |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the refund was created in our system |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the refund was last updated |  |
| **idempotencyKey** | **kotlin.String** | Client-generated key to prevent duplicate refunds |  [optional] |
| **provider** | **kotlin.String** | The payment provider used |  [optional] |
| **reason** | **kotlin.String** | Reason for the refund |  [optional] |
| **referenceValue** | **kotlin.String** | Acquirer Reference Number (ARN) or tracking number |  [optional] |
| **providerCreatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the refund was processed by the provider |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | pending, succeeded, failed, canceled |



