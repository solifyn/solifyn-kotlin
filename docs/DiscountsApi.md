# DiscountsApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**discountsCreate**](DiscountsApi.md#discountsCreate) | **POST** /v1/discounts | Create Discount |
| [**discountsDelete**](DiscountsApi.md#discountsDelete) | **DELETE** /v1/discounts/{id} | Delete Discount |
| [**discountsGet**](DiscountsApi.md#discountsGet) | **GET** /v1/discounts/{id} | Retrieve Discount |
| [**discountsList**](DiscountsApi.md#discountsList) | **GET** /v1/discounts | List Discounts |
| [**discountsUpdate**](DiscountsApi.md#discountsUpdate) | **PATCH** /v1/discounts/{id} | Update Discount |
| [**discountsValidate**](DiscountsApi.md#discountsValidate) | **GET** /v1/discounts/validate | Validate Code |


<a id="discountsCreate"></a>
# **discountsCreate**
> Discount discountsCreate(discountCreate)

Create Discount

Create a new discount code within your active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DiscountsApi()
val discountCreate : DiscountCreate =  // DiscountCreate | 
try {
    val result : Discount = apiInstance.discountsCreate(discountCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DiscountsApi#discountsCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DiscountsApi#discountsCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **discountCreate** | [**DiscountCreate**](DiscountCreate.md)|  | |

### Return type

[**Discount**](Discount.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="discountsDelete"></a>
# **discountsDelete**
> LicensesDeactivate200Response discountsDelete(id)

Delete Discount

Delete a specific discount code by ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DiscountsApi()
val id : kotlin.String = disc_123 // kotlin.String | The unique discount ID.
try {
    val result : LicensesDeactivate200Response = apiInstance.discountsDelete(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DiscountsApi#discountsDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DiscountsApi#discountsDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique discount ID. | |

### Return type

[**LicensesDeactivate200Response**](LicensesDeactivate200Response.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="discountsGet"></a>
# **discountsGet**
> Discount discountsGet(id)

Retrieve Discount

Retrieve details of a specific discount code using its ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DiscountsApi()
val id : kotlin.String = disc_123 // kotlin.String | The unique discount ID.
try {
    val result : Discount = apiInstance.discountsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DiscountsApi#discountsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DiscountsApi#discountsGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique discount ID. | |

### Return type

[**Discount**](Discount.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="discountsList"></a>
# **discountsList**
> DiscountsList200Response discountsList(sorting, limit, page, query, id)

List Discounts

List and query discounts belonging to your active business with support for fuzzy search by code, pagination, and sorting.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DiscountsApi()
val sorting : kotlin.String = sorting_example // kotlin.String | Sorting criterion. Add a minus sign - before the criteria name to sort by descending order.
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Size of a page, defaults to 10. Maximum is 100.
val page : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Page number, defaults to 1.
val query : kotlin.String = query_example // kotlin.String | Filter by discount code (fuzzy, case-insensitive).
val id : kotlin.String = id_example // kotlin.String | Filter by discount ID.
try {
    val result : DiscountsList200Response = apiInstance.discountsList(sorting, limit, page, query, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DiscountsApi#discountsList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DiscountsApi#discountsList")
    e.printStackTrace()
}
```

### Parameters
| **sorting** | **kotlin.String**| Sorting criterion. Add a minus sign - before the criteria name to sort by descending order. | [optional] [enum: created_at, -created_at] |
| **limit** | **java.math.BigDecimal**| Size of a page, defaults to 10. Maximum is 100. | [optional] [default to 10] |
| **page** | **java.math.BigDecimal**| Page number, defaults to 1. | [optional] [default to 1] |
| **query** | **kotlin.String**| Filter by discount code (fuzzy, case-insensitive). | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Filter by discount ID. | [optional] |

### Return type

[**DiscountsList200Response**](DiscountsList200Response.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="discountsUpdate"></a>
# **discountsUpdate**
> Discount discountsUpdate(id, discountUpdate)

Update Discount

Update details of an existing discount code.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DiscountsApi()
val id : kotlin.String = disc_123 // kotlin.String | The unique discount ID.
val discountUpdate : DiscountUpdate =  // DiscountUpdate | 
try {
    val result : Discount = apiInstance.discountsUpdate(id, discountUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DiscountsApi#discountsUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DiscountsApi#discountsUpdate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique discount ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **discountUpdate** | [**DiscountUpdate**](DiscountUpdate.md)|  | |

### Return type

[**Discount**](Discount.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="discountsValidate"></a>
# **discountsValidate**
> Discount discountsValidate(code, businessId)

Validate Code

Validate if a specific discount code is active and valid for purchase checkout.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DiscountsApi()
val code : kotlin.String = SAVE20 // kotlin.String | The plain discount code string
val businessId : kotlin.String = biz_123 // kotlin.String | The business database ID context
try {
    val result : Discount = apiInstance.discountsValidate(code, businessId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DiscountsApi#discountsValidate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DiscountsApi#discountsValidate")
    e.printStackTrace()
}
```

### Parameters
| **code** | **kotlin.String**| The plain discount code string | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **businessId** | **kotlin.String**| The business database ID context | |

### Return type

[**Discount**](Discount.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

