
# LicensesCreateRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **productId** | [**java.util.UUID**](java.util.UUID.md) | The unique product identifier (internal product ID or ID) for which the license key will be issued. |  |
| **customerId** | **kotlin.String** | The unique customer identifier (internal customer ID or ID) who will own this license key. |  |
| **activationLimit** | **kotlin.Int** | The maximum number of concurrent device or server activations allowed for this license key. |  [optional] |
| **expiryHours** | **kotlin.Int** | Relative validity period of the license in hours starting from the time of creation. |  [optional] |
| **key** | **kotlin.String** | Optional custom license key string. If not provided, a random uppercase cryptographic serial key (e.g., ABCD-EFGH) will be generated automatically. |  [optional] |



