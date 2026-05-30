
# Order

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Unique internal database identifier. |  |
| **invoiceUrl** | **kotlin.String** | The invoice print URL. |  |
| **customer** | [**OrderCustomer**](OrderCustomer.md) | Customer details. |  |
| **totalAmount** | **kotlin.Int** | Total paid amount in cents. |  |
| **subtotal** | **kotlin.Int** | Subtotal amount in cents. |  |
| **taxAmount** | **kotlin.Int** | Tax amount in cents. |  |
| **applicationFee** | **kotlin.Int** | Application fee in cents. |  |
| **amountAfterFees** | **kotlin.Int** | Net amount after fees in cents. |  |
| **currency** | **kotlin.String** | Currency code. |  |
| **status** | **kotlin.String** | Current status of the payment. |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Payment creation timestamp. |  |
| **paymentMethod** | **kotlin.String** | Payment method utilized. |  |
| **productCart** | [**kotlin.collections.List&lt;OrderProductCart&gt;**](OrderProductCart.md) | Products purchased in this order. |  |
| **refundable** | **kotlin.Boolean** | Indicates whether the order is eligible for refund. |  |
| **businessId** | **kotlin.String** | Business unique ID identifier. |  |
| **businessName** | **kotlin.String** | Business display title/name. |  |
| **paidAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Payment completion/paid timestamp. |  [optional] |
| **cardLastFour** | **kotlin.String** | Last four digits of card used. |  [optional] |
| **cardNetwork** | **kotlin.String** | Card network/brand. |  [optional] |
| **cardType** | **kotlin.String** | Card type. |  [optional] |
| **billing** | [**OrderBilling**](OrderBilling.md) | Billing address details. |  [optional] |
| **metadata** | [**kotlin.Any**](.md) | Custom metadata payload associated with this payment. |  [optional] |
| **order** | [**OrderDetail**](OrderDetail.md) | Order details snapshot. |  [optional] |
| **refunds** | [**kotlin.collections.List&lt;OrderRefund&gt;**](OrderRefund.md) | List of refunds associated with this payment. |  [optional] |
| **billingReason** | **kotlin.String** | Billing reason detail. |  [optional] |



