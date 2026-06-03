
# WebhookPaymentPayload

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Internal payment ID. |  [optional] |
| **status** | **kotlin.String** |  |  [optional] |
| **substatus** | **kotlin.String** |  |  [optional] |
| **customerId** | **kotlin.String** |  |  [optional] |
| **customerEmail** | **kotlin.String** |  |  [optional] |
| **customerName** | **kotlin.String** |  |  [optional] |
| **customerUsername** | **kotlin.String** |  |  [optional] |
| **productTitle** | **kotlin.String** |  |  [optional] |
| **productRoute** | **kotlin.String** |  |  [optional] |
| **planId** | **kotlin.String** |  |  [optional] |
| **membershipId** | **kotlin.String** |  |  [optional] |
| **membershipStatus** | **kotlin.String** |  |  [optional] |
| **billingReason** | **kotlin.String** |  |  [optional] |
| **amount** | **kotlin.String** | Dollar value, 2 d.p. |  [optional] |
| **subtotal** | **kotlin.String** |  |  [optional] |
| **usdTotal** | **kotlin.String** |  |  [optional] |
| **feeAmount** | **kotlin.String** |  |  [optional] |
| **amountAfterFees** | **kotlin.String** |  |  [optional] |
| **taxAmount** | **kotlin.String** |  |  [optional] |
| **taxBehavior** | **kotlin.String** |  |  [optional] |
| **taxRefundedAmount** | **kotlin.String** |  |  [optional] |
| **refundedAmount** | **kotlin.String** |  |  [optional] |
| **settlementAmount** | **kotlin.String** |  |  [optional] |
| **settlementCurrency** | **kotlin.String** |  |  [optional] |
| **settlementExchangeRate** | **kotlin.String** |  |  [optional] |
| **currency** | **kotlin.String** |  |  [optional] |
| **refundable** | **kotlin.Boolean** |  |  [optional] |
| **retryable** | **kotlin.Boolean** |  |  [optional] |
| **autoRefunded** | **kotlin.Boolean** |  |  [optional] |
| **paymentMethod** | **kotlin.String** |  |  [optional] |
| **cardBrand** | **kotlin.String** |  |  [optional] |
| **cardLast4** | **kotlin.String** |  |  [optional] |
| **cardExpMonth** | **kotlin.Int** |  |  [optional] |
| **cardExpYear** | **kotlin.Int** |  |  [optional] |
| **billingAddress** | [**WebhookPaymentPayloadBillingAddress**](WebhookPaymentPayloadBillingAddress.md) |  |  [optional] |
| **licenseKey** | **kotlin.String** |  |  [optional] |
| **filesSnapshot** | [**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md) |  |  [optional] |
| **checkoutId** | **kotlin.String** |  |  [optional] |
| **discountCode** | **kotlin.String** |  |  [optional] |
| **failureMessage** | **kotlin.String** |  |  [optional] |
| **paidAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **refundedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **disputeAlertedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **lastPaymentAttempt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **nextPaymentAttempt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **paymentEventType** | **kotlin.String** |  |  [optional] |
| **lastEventType** | **kotlin.String** |  |  [optional] |
| **businessId** | **kotlin.String** |  |  [optional] |



