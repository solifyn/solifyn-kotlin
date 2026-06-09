# CheckoutLinksApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**checkoutLinksCreate**](CheckoutLinksApi.md#checkoutLinksCreate) | **POST** /v1/checkout-links | Create Checkout Link |
| [**checkoutLinksDelete**](CheckoutLinksApi.md#checkoutLinksDelete) | **DELETE** /v1/checkout-links/{id} | Delete Checkout Link |
| [**checkoutLinksGet**](CheckoutLinksApi.md#checkoutLinksGet) | **GET** /v1/checkout-links/{id} | Retrieve Checkout Link Details |
| [**checkoutLinksList**](CheckoutLinksApi.md#checkoutLinksList) | **GET** /v1/checkout-links | List Checkout Links |
| [**checkoutLinksUpdate**](CheckoutLinksApi.md#checkoutLinksUpdate) | **PATCH** /v1/checkout-links/{id} | Update Checkout Link |


<a id="checkoutLinksCreate"></a>
# **checkoutLinksCreate**
> CheckoutLinkResponseDto checkoutLinksCreate(createCheckoutLinkDto)

Create Checkout Link

Generate a new checkout session link.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutLinksApi()
val createCheckoutLinkDto : CreateCheckoutLinkDto =  // CreateCheckoutLinkDto | 
try {
    val result : CheckoutLinkResponseDto = apiInstance.checkoutLinksCreate(createCheckoutLinkDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutLinksApi#checkoutLinksCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutLinksApi#checkoutLinksCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createCheckoutLinkDto** | [**CreateCheckoutLinkDto**](CreateCheckoutLinkDto.md)|  | |

### Return type

[**CheckoutLinkResponseDto**](CheckoutLinkResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="checkoutLinksDelete"></a>
# **checkoutLinksDelete**
> CheckoutLinkMessageResponseDto checkoutLinksDelete(id)

Delete Checkout Link

Permanently remove a checkout link.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutLinksApi()
val id : kotlin.String = chk_123 // kotlin.String | Checkout Link ID
try {
    val result : CheckoutLinkMessageResponseDto = apiInstance.checkoutLinksDelete(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutLinksApi#checkoutLinksDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutLinksApi#checkoutLinksDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Checkout Link ID | |

### Return type

[**CheckoutLinkMessageResponseDto**](CheckoutLinkMessageResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="checkoutLinksGet"></a>
# **checkoutLinksGet**
> CheckoutLinkResponseDto checkoutLinksGet(id)

Retrieve Checkout Link Details

Get details of a specific checkout link by ID (public access).

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutLinksApi()
val id : kotlin.String = chk_123 // kotlin.String | Checkout Link ID
try {
    val result : CheckoutLinkResponseDto = apiInstance.checkoutLinksGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutLinksApi#checkoutLinksGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutLinksApi#checkoutLinksGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Checkout Link ID | |

### Return type

[**CheckoutLinkResponseDto**](CheckoutLinkResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="checkoutLinksList"></a>
# **checkoutLinksList**
> kotlin.collections.List&lt;CheckoutLinkResponseDto&gt; checkoutLinksList()

List Checkout Links

Retrieve all active checkout session links for the active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutLinksApi()
try {
    val result : kotlin.collections.List<CheckoutLinkResponseDto> = apiInstance.checkoutLinksList()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutLinksApi#checkoutLinksList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutLinksApi#checkoutLinksList")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CheckoutLinkResponseDto&gt;**](CheckoutLinkResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="checkoutLinksUpdate"></a>
# **checkoutLinksUpdate**
> CheckoutLinkMessageResponseDto checkoutLinksUpdate(id, updateCheckoutLinkDto)

Update Checkout Link

Update title, custom pricing, redirection URLs, or friendly inputs for a checkout link.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CheckoutLinksApi()
val id : kotlin.String = chk_123 // kotlin.String | Checkout Link ID
val updateCheckoutLinkDto : UpdateCheckoutLinkDto =  // UpdateCheckoutLinkDto | 
try {
    val result : CheckoutLinkMessageResponseDto = apiInstance.checkoutLinksUpdate(id, updateCheckoutLinkDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutLinksApi#checkoutLinksUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutLinksApi#checkoutLinksUpdate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Checkout Link ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateCheckoutLinkDto** | [**UpdateCheckoutLinkDto**](UpdateCheckoutLinkDto.md)|  | |

### Return type

[**CheckoutLinkMessageResponseDto**](CheckoutLinkMessageResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

