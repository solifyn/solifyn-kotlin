# ProductsApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**productsArchive**](ProductsApi.md#productsArchive) | **DELETE** /v1/products/{id} | Archive Product |
| [**productsCreate**](ProductsApi.md#productsCreate) | **POST** /v1/products | Create Product |
| [**productsGet**](ProductsApi.md#productsGet) | **GET** /v1/products/{id} | Retrieve Product |
| [**productsList**](ProductsApi.md#productsList) | **GET** /v1/products | List Products |
| [**productsUnarchive**](ProductsApi.md#productsUnarchive) | **POST** /v1/products/{id}/unarchive | Unarchive Product |
| [**productsUpdate**](ProductsApi.md#productsUpdate) | **PATCH** /v1/products/{id} | Update Product |


<a id="productsArchive"></a>
# **productsArchive**
> ProductsArchive200Response productsArchive(id)

Archive Product

Archive a specific product to hide it from checkout pages and search results. Products are soft-deleted (archived) and can be restored using the unarchive endpoint.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductsApi()
val id : kotlin.String = prod_123 // kotlin.String | The unique product ID to archive.
try {
    val result : ProductsArchive200Response = apiInstance.productsArchive(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#productsArchive")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#productsArchive")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique product ID to archive. | |

### Return type

[**ProductsArchive200Response**](ProductsArchive200Response.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="productsCreate"></a>
# **productsCreate**
> Product productsCreate(productCreate)

Create Product

Create a new product within your active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductsApi()
val productCreate : ProductCreate =  // ProductCreate | 
try {
    val result : Product = apiInstance.productsCreate(productCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#productsCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#productsCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productCreate** | [**ProductCreate**](ProductCreate.md)|  | |

### Return type

[**Product**](Product.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="productsGet"></a>
# **productsGet**
> Product productsGet(id)

Retrieve Product

Retrieve details of a specific product using its ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductsApi()
val id : kotlin.String = prod_123 // kotlin.String | The unique product ID.
try {
    val result : Product = apiInstance.productsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#productsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#productsGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique product ID. | |

### Return type

[**Product**](Product.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="productsList"></a>
# **productsList**
> ProductsList200Response productsList(pricingType, sorting, limit, page, isRecurring, isArchived, query, id)

List Products

List and query products belonging to your active business with support for fuzzy search, filters, pagination, and sorting.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductsApi()
val pricingType : kotlin.String = pricingType_example // kotlin.String | Filter by pricing type.
val sorting : kotlin.String = sorting_example // kotlin.String | Sorting criterion. Add a minus sign - before the criteria name to sort by descending order.
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Size of a page, defaults to 10. Maximum is 100.
val page : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Page number, defaults to 1.
val isRecurring : kotlin.Boolean = true // kotlin.Boolean | Filter on recurring products (subscriptions). If true, only subscription tiers are returned. If false, only one-time purchase products are returned.
val isArchived : kotlin.Boolean = true // kotlin.Boolean | Filter by archived status.
val query : kotlin.String = query_example // kotlin.String | Filter by product name (fuzzy, case-insensitive).
val id : kotlin.String = id_example // kotlin.String | Filter by product ID.
try {
    val result : ProductsList200Response = apiInstance.productsList(pricingType, sorting, limit, page, isRecurring, isArchived, query, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#productsList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#productsList")
    e.printStackTrace()
}
```

### Parameters
| **pricingType** | **kotlin.String**| Filter by pricing type. | [optional] |
| **sorting** | **kotlin.String**| Sorting criterion. Add a minus sign - before the criteria name to sort by descending order. | [optional] [enum: created_at, -created_at, name, -name, price_amount, -price_amount] |
| **limit** | **java.math.BigDecimal**| Size of a page, defaults to 10. Maximum is 100. | [optional] [default to 10] |
| **page** | **java.math.BigDecimal**| Page number, defaults to 1. | [optional] [default to 1] |
| **isRecurring** | **kotlin.Boolean**| Filter on recurring products (subscriptions). If true, only subscription tiers are returned. If false, only one-time purchase products are returned. | [optional] |
| **isArchived** | **kotlin.Boolean**| Filter by archived status. | [optional] |
| **query** | **kotlin.String**| Filter by product name (fuzzy, case-insensitive). | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Filter by product ID. | [optional] |

### Return type

[**ProductsList200Response**](ProductsList200Response.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="productsUnarchive"></a>
# **productsUnarchive**
> ProductsUnarchive200Response productsUnarchive(id)

Unarchive Product

Restore an archived product back to active status, making it visible again.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductsApi()
val id : kotlin.String = prod_123 // kotlin.String | The unique product ID to unarchive.
try {
    val result : ProductsUnarchive200Response = apiInstance.productsUnarchive(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#productsUnarchive")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#productsUnarchive")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique product ID to unarchive. | |

### Return type

[**ProductsUnarchive200Response**](ProductsUnarchive200Response.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="productsUpdate"></a>
# **productsUpdate**
> ProductMessageResponseDto productsUpdate(id, productUpdate)

Update Product

Update details of an existing product.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = ProductsApi()
val id : kotlin.String = prod_123 // kotlin.String | The unique product ID.
val productUpdate : ProductUpdate =  // ProductUpdate | 
try {
    val result : ProductMessageResponseDto = apiInstance.productsUpdate(id, productUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#productsUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#productsUpdate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique product ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productUpdate** | [**ProductUpdate**](ProductUpdate.md)|  | |

### Return type

[**ProductMessageResponseDto**](ProductMessageResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

