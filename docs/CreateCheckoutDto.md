
# CreateCheckoutDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **productId** | **kotlin.String** | The public product identifier (product ID) |  |
| **currency** | **kotlin.String** | Three-letter ISO currency code (lowercase) |  [optional] |
| **quantity** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The quantity of items to buy |  [optional] |
| **discountCode** | **kotlin.String** | Discount code to apply |  [optional] |
| **customPrice** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Custom price paid by customer (for Pay What You Want products) |  [optional] |
| **customerEmail** | **kotlin.String** | Email address of the customer |  [optional] |
| **checkoutData** | [**kotlin.Any**](.md) | JSON metadata or checkout custom information |  [optional] |
| **customFields** | [**kotlin.Any**](.md) | Custom text fields required for the purchase |  [optional] |
| **aff** | **kotlin.String** | Affiliate partner tracking code |  [optional] |
| **checkoutId** | **kotlin.String** | The existing checkout database ID to validate / update |  [optional] |



