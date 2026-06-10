# CheckoutApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**checkoutCreate**](CheckoutApi.md#checkoutCreate) | **POST** /v1/checkout/create | Create Checkout Session |
| [**checkoutCreateCollection**](CheckoutApi.md#checkoutCreateCollection) | **POST** /v1/checkout/collection/create | Create Collection Checkout Session |
| [**checkoutCreateSetup**](CheckoutApi.md#checkoutCreateSetup) | **POST** /v1/checkout/setup-configuration | Create Setup Checkout Configuration |
| [**checkoutGetSession**](CheckoutApi.md#checkoutGetSession) | **GET** /v1/checkout/session/{id} | Get Checkout Session Details |
| [**checkoutPricePreview**](CheckoutApi.md#checkoutPricePreview) | **GET** /v1/checkout/price-preview | Get Converted Price Preview |
| [**checkoutSupportedCurrencies**](CheckoutApi.md#checkoutSupportedCurrencies) | **GET** /v1/checkout/supported-currencies | Get Supported Currencies |


<a id="checkoutCreate"></a>
# **checkoutCreate**
> CheckoutResponseDto checkoutCreate(createCheckoutDto)

Create Checkout Session

Create a new payment configuration for a product. Returns redirect URLs pointing to the custom checkout layout.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutApi()
val createCheckoutDto : CreateCheckoutDto =  // CreateCheckoutDto | 
try {
    val result : CheckoutResponseDto = apiInstance.checkoutCreate(createCheckoutDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#checkoutCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#checkoutCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createCheckoutDto** | [**CreateCheckoutDto**](CreateCheckoutDto.md)|  | |

### Return type

[**CheckoutResponseDto**](CheckoutResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="checkoutCreateCollection"></a>
# **checkoutCreateCollection**
> CheckoutResponseDto checkoutCreateCollection(createCollectionCheckoutDto)

Create Collection Checkout Session

Create a new payment configuration for a product bundle/collection.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutApi()
val createCollectionCheckoutDto : CreateCollectionCheckoutDto =  // CreateCollectionCheckoutDto | 
try {
    val result : CheckoutResponseDto = apiInstance.checkoutCreateCollection(createCollectionCheckoutDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#checkoutCreateCollection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#checkoutCreateCollection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createCollectionCheckoutDto** | [**CreateCollectionCheckoutDto**](CreateCollectionCheckoutDto.md)|  | |

### Return type

[**CheckoutResponseDto**](CheckoutResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="checkoutCreateSetup"></a>
# **checkoutCreateSetup**
> checkoutCreateSetup(createSetupCheckoutDto)

Create Setup Checkout Configuration

Create a new checkout session in setup mode for collecting cards without immediate charge.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutApi()
val createSetupCheckoutDto : CreateSetupCheckoutDto =  // CreateSetupCheckoutDto | 
try {
    apiInstance.checkoutCreateSetup(createSetupCheckoutDto)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#checkoutCreateSetup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#checkoutCreateSetup")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createSetupCheckoutDto** | [**CreateSetupCheckoutDto**](CreateSetupCheckoutDto.md)|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="checkoutGetSession"></a>
# **checkoutGetSession**
> CheckoutSessionDetailsDto checkoutGetSession(id)

Get Checkout Session Details

Retrieve checkout details to mount the custom embedded checkout.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutApi()
val id : kotlin.String = ch_XXXXXXXXXXX // kotlin.String | Internal database checkout session ID
try {
    val result : CheckoutSessionDetailsDto = apiInstance.checkoutGetSession(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#checkoutGetSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#checkoutGetSession")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Internal database checkout session ID | |

### Return type

[**CheckoutSessionDetailsDto**](CheckoutSessionDetailsDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="checkoutPricePreview"></a>
# **checkoutPricePreview**
> PricePreviewResponseDto checkoutPricePreview(productId, addons, currency, discount, qty, customPrice)

Get Converted Price Preview

Pre-calculate target currencies, applied discounts, and PWYW values before mounting the checkout.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutApi()
val productId : kotlin.String = prod_z2o92kEl6cYYX // kotlin.String | Public product ID
val addons : kotlin.String = addons_example // kotlin.String | 
val currency : kotlin.String = vnd // kotlin.String | Target currency code (ISO)
val discount : kotlin.String = 10 // kotlin.String | Percentage discount rate
val qty : kotlin.String = 1 // kotlin.String | Number of product units
val customPrice : kotlin.String = 15 // kotlin.String | Override price for PWYW products
try {
    val result : PricePreviewResponseDto = apiInstance.checkoutPricePreview(productId, addons, currency, discount, qty, customPrice)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#checkoutPricePreview")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#checkoutPricePreview")
    e.printStackTrace()
}
```

### Parameters
| **productId** | **kotlin.String**| Public product ID | |
| **addons** | **kotlin.String**|  | |
| **currency** | **kotlin.String**| Target currency code (ISO) | [optional] |
| **discount** | **kotlin.String**| Percentage discount rate | [optional] |
| **qty** | **kotlin.String**| Number of product units | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customPrice** | **kotlin.String**| Override price for PWYW products | [optional] |

### Return type

[**PricePreviewResponseDto**](PricePreviewResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="checkoutSupportedCurrencies"></a>
# **checkoutSupportedCurrencies**
> kotlin.collections.List&lt;SupportedCurrenciesResponseDto&gt; checkoutSupportedCurrencies()

Get Supported Currencies

Retrieve all currencies supported for payouts and conversions.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutApi()
try {
    val result : kotlin.collections.List<SupportedCurrenciesResponseDto> = apiInstance.checkoutSupportedCurrencies()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#checkoutSupportedCurrencies")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#checkoutSupportedCurrencies")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;SupportedCurrenciesResponseDto&gt;**](SupportedCurrenciesResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

