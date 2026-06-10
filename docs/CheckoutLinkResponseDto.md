
# CheckoutLinkResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) | The checkout link ID |  |
| **quantity** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Quantity to purchase |  |
| **showDiscounts** | **kotlin.Boolean** | Whether to show discounts on the checkout page |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the link was created |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the link was last updated |  |
| **title** | **kotlin.String** | The title of the checkout link |  [optional] |
| **productId** | **kotlin.String** | The linked Product ID |  [optional] |
| **collectionId** | **kotlin.String** | The linked Collection ID |  [optional] |
| **customerName** | **kotlin.String** | Pre-filled customer name |  [optional] |
| **customerEmail** | **kotlin.String** | Pre-filled customer email |  [optional] |
| **addressLine1** | **kotlin.String** | Pre-filled address line 1 |  [optional] |
| **city** | **kotlin.String** | Pre-filled city |  [optional] |
| **state** | **kotlin.String** | Pre-filled state |  [optional] |
| **postalCode** | **kotlin.String** | Pre-filled postal code |  [optional] |
| **country** | **kotlin.String** | Pre-filled country |  [optional] |
| **redirectUrl** | **kotlin.String** | URL to redirect to after successful payment |  [optional] |
| **cancelUrl** | **kotlin.String** | URL to redirect to if payment is cancelled |  [optional] |



