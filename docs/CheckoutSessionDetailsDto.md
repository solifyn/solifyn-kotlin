
# CheckoutSessionDetailsDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Checkout session identifier |  |
| **price** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Total purchase amount |  |
| **currency** | **kotlin.String** | ISO currency code of the purchase |  |
| **storeName** | **kotlin.String** | Title or name of the merchant/store selling the item |  |
| **status** | **kotlin.String** | Current status of the checkout session |  |
| **billingAddress** | [**kotlin.Any**](.md) | Customer billing address details |  [optional] |
| **customFields** | [**kotlin.Any**](.md) | Custom fields collected during purchase |  [optional] |
| **sessionId** | **kotlin.String** | The payment partner session ID |  [optional] |
| **paymentId** | **kotlin.String** | Database payment transaction ID |  [optional] |
| **checkoutUrl** | **kotlin.String** | Checkout session redirect URL if loaded in link mode |  [optional] |
| **product** | [**Product**](Product.md) | The details of the product being purchased |  [optional] |
| **entitlementGrants** | [**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md) | List of entitlement grants (e.g. GitHub repo invites) associated with this checkout. |  [optional] |



