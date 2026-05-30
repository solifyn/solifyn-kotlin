# ProductAddOnsApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**productsCreateAddon**](ProductAddOnsApi.md#productsCreateAddon) | **POST** /v1/products/{id}/addons | Create Product Add-on |
| [**productsDeleteAddon**](ProductAddOnsApi.md#productsDeleteAddon) | **DELETE** /v1/products/{id}/addons/{addonId} | Delete Product Add-on |
| [**productsGetAddon**](ProductAddOnsApi.md#productsGetAddon) | **GET** /v1/products/{id}/addons/{addonId} | Retrieve Product Add-on |
| [**productsListAddons**](ProductAddOnsApi.md#productsListAddons) | **GET** /v1/products/{id}/addons | List Product Add-ons |
| [**productsListAllAddons**](ProductAddOnsApi.md#productsListAllAddons) | **GET** /v1/products/all-addons/list | List All Add-ons |
| [**productsUpdateAddon**](ProductAddOnsApi.md#productsUpdateAddon) | **PATCH** /v1/products/{id}/addons/{addonId} | Update Product Add-on |


<a id="productsCreateAddon"></a>
# **productsCreateAddon**
> Addon productsCreateAddon(id, addonCreate)

Create Product Add-on

Attach a new add-on configuration to a product.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductAddOnsApi()
val id : kotlin.String = prod_parent_123 // kotlin.String | The parent product ID.
val addonCreate : AddonCreate =  // AddonCreate | 
try {
    val result : Addon = apiInstance.productsCreateAddon(id, addonCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductAddOnsApi#productsCreateAddon")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAddOnsApi#productsCreateAddon")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The parent product ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **addonCreate** | [**AddonCreate**](AddonCreate.md)|  | |

### Return type

[**Addon**](Addon.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="productsDeleteAddon"></a>
# **productsDeleteAddon**
> ProductMessageResponseDto productsDeleteAddon(id, addonId)

Delete Product Add-on

Remove an add-on configuration from a product.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductAddOnsApi()
val id : kotlin.String = prod_parent_123 // kotlin.String | The parent product ID.
val addonId : kotlin.String = prod_addon_123 // kotlin.String | The add-on product ID to remove.
try {
    val result : ProductMessageResponseDto = apiInstance.productsDeleteAddon(id, addonId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductAddOnsApi#productsDeleteAddon")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAddOnsApi#productsDeleteAddon")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The parent product ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **addonId** | **kotlin.String**| The add-on product ID to remove. | |

### Return type

[**ProductMessageResponseDto**](ProductMessageResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="productsGetAddon"></a>
# **productsGetAddon**
> Addon productsGetAddon(id, addonId)

Retrieve Product Add-on

Retrieve a specific add-on configuration of a product.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductAddOnsApi()
val id : kotlin.String = prod_parent_123 // kotlin.String | The parent product ID.
val addonId : kotlin.String = prod_addon_123 // kotlin.String | The add-on product ID.
try {
    val result : Addon = apiInstance.productsGetAddon(id, addonId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductAddOnsApi#productsGetAddon")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAddOnsApi#productsGetAddon")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The parent product ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **addonId** | **kotlin.String**| The add-on product ID. | |

### Return type

[**Addon**](Addon.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="productsListAddons"></a>
# **productsListAddons**
> kotlin.collections.List&lt;Addon&gt; productsListAddons(id)

List Product Add-ons

Retrieve all add-on configurations attached to a product.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductAddOnsApi()
val id : kotlin.String = prod_parent_123 // kotlin.String | The parent product ID.
try {
    val result : kotlin.collections.List<Addon> = apiInstance.productsListAddons(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductAddOnsApi#productsListAddons")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAddOnsApi#productsListAddons")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The parent product ID. | |

### Return type

[**kotlin.collections.List&lt;Addon&gt;**](Addon.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="productsListAllAddons"></a>
# **productsListAllAddons**
> productsListAllAddons()

List All Add-ons

Retrieve all configured add-on configurations for the active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductAddOnsApi()
try {
    apiInstance.productsListAllAddons()
} catch (e: ClientException) {
    println("4xx response calling ProductAddOnsApi#productsListAllAddons")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAddOnsApi#productsListAllAddons")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="productsUpdateAddon"></a>
# **productsUpdateAddon**
> Addon productsUpdateAddon(id, addonId, addonUpdate)

Update Product Add-on

Update an existing add-on configuration for a product.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductAddOnsApi()
val id : kotlin.String = prod_parent_123 // kotlin.String | The parent product ID.
val addonId : kotlin.String = prod_addon_123 // kotlin.String | The add-on product ID.
val addonUpdate : AddonUpdate =  // AddonUpdate | 
try {
    val result : Addon = apiInstance.productsUpdateAddon(id, addonId, addonUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductAddOnsApi#productsUpdateAddon")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAddOnsApi#productsUpdateAddon")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The parent product ID. | |
| **addonId** | **kotlin.String**| The add-on product ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **addonUpdate** | [**AddonUpdate**](AddonUpdate.md)|  | |

### Return type

[**Addon**](Addon.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

