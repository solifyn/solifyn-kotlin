
# CreateCheckoutLinkDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **productId** | **kotlin.String** | Product database/Whop ID to sell |  |
| **title** | **kotlin.String** | The friendly display title of this checkout link |  [optional] |
| **collectionId** | **kotlin.String** | Optional collection database ID to sell |  [optional] |
| **customerName** | **kotlin.String** | Prefilled customer name for checkout inputs |  [optional] |
| **customerEmail** | **kotlin.String** | Prefilled customer email for checkout inputs |  [optional] |
| **addressLine1** | **kotlin.String** | Prefilled customer billing address line 1 |  [optional] |
| **city** | **kotlin.String** | Prefilled customer billing city |  [optional] |
| **state** | **kotlin.String** | Prefilled customer billing state |  [optional] |
| **postalCode** | **kotlin.String** | Prefilled customer billing zip/postal code |  [optional] |
| **country** | **kotlin.String** | Prefilled customer billing country (2-letter ISO) |  [optional] |
| **quantity** | [**kotlin.Any**](.md) | Override quantity for checkout session |  [optional] |
| **redirectUrl** | **kotlin.String** | The absolute URL to redirect to upon successful payment completion |  [optional] |
| **cancelUrl** | **kotlin.String** | The absolute URL to redirect to if a customer cancels the payment |  [optional] |
| **showDiscounts** | **kotlin.Boolean** | Whether to display discount input form fields on checkout screen |  [optional] |



