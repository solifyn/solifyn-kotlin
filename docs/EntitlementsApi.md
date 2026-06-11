# EntitlementsApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**entitlementsCreate**](EntitlementsApi.md#entitlementsCreate) | **POST** /v1/entitlements | Create Entitlement |
| [**entitlementsDelete**](EntitlementsApi.md#entitlementsDelete) | **DELETE** /v1/entitlements/{id} | Delete Entitlement |
| [**entitlementsGet**](EntitlementsApi.md#entitlementsGet) | **GET** /v1/entitlements/{id} | Retrieve Entitlement |
| [**entitlementsList**](EntitlementsApi.md#entitlementsList) | **GET** /v1/entitlements | List Entitlements |
| [**entitlementsUpdate**](EntitlementsApi.md#entitlementsUpdate) | **PATCH** /v1/entitlements/{id} | Update Entitlement |


<a id="entitlementsCreate"></a>
# **entitlementsCreate**
> EntitlementDetailResponseDto entitlementsCreate(createEntitlementDto)

Create Entitlement

Create a new independent access entitlement.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = EntitlementsApi()
val createEntitlementDto : CreateEntitlementDto =  // CreateEntitlementDto | 
try {
    val result : EntitlementDetailResponseDto = apiInstance.entitlementsCreate(createEntitlementDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EntitlementsApi#entitlementsCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EntitlementsApi#entitlementsCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createEntitlementDto** | [**CreateEntitlementDto**](CreateEntitlementDto.md)|  | |

### Return type

[**EntitlementDetailResponseDto**](EntitlementDetailResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="entitlementsDelete"></a>
# **entitlementsDelete**
> EntitlementDetailResponseDto entitlementsDelete(id)

Delete Entitlement

Delete an independent entitlement and unlink all mapped products.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = EntitlementsApi()
val id : kotlin.String = ent_8Z1aB2cD3eF4gH5iJ6kL7m // kotlin.String | The unique entitlement ID.
try {
    val result : EntitlementDetailResponseDto = apiInstance.entitlementsDelete(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EntitlementsApi#entitlementsDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EntitlementsApi#entitlementsDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique entitlement ID. | |

### Return type

[**EntitlementDetailResponseDto**](EntitlementDetailResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="entitlementsGet"></a>
# **entitlementsGet**
> EntitlementDetailResponseDto entitlementsGet(id)

Retrieve Entitlement

Retrieve a specific entitlement definition by ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = EntitlementsApi()
val id : kotlin.String = ent_8Z1aB2cD3eF4gH5iJ6kL7m // kotlin.String | The unique entitlement ID.
try {
    val result : EntitlementDetailResponseDto = apiInstance.entitlementsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EntitlementsApi#entitlementsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EntitlementsApi#entitlementsGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique entitlement ID. | |

### Return type

[**EntitlementDetailResponseDto**](EntitlementDetailResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="entitlementsList"></a>
# **entitlementsList**
> kotlin.collections.List&lt;EntitlementDetailResponseDto&gt; entitlementsList()

List Entitlements

List all independent entitlements for the active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = EntitlementsApi()
try {
    val result : kotlin.collections.List<EntitlementDetailResponseDto> = apiInstance.entitlementsList()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EntitlementsApi#entitlementsList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EntitlementsApi#entitlementsList")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;EntitlementDetailResponseDto&gt;**](EntitlementDetailResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="entitlementsUpdate"></a>
# **entitlementsUpdate**
> EntitlementDetailResponseDto entitlementsUpdate(id, updateEntitlementDto)

Update Entitlement

Update details of an existing independent entitlement.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = EntitlementsApi()
val id : kotlin.String = ent_8Z1aB2cD3eF4gH5iJ6kL7m // kotlin.String | The unique entitlement ID.
val updateEntitlementDto : UpdateEntitlementDto =  // UpdateEntitlementDto | 
try {
    val result : EntitlementDetailResponseDto = apiInstance.entitlementsUpdate(id, updateEntitlementDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EntitlementsApi#entitlementsUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EntitlementsApi#entitlementsUpdate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique entitlement ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateEntitlementDto** | [**UpdateEntitlementDto**](UpdateEntitlementDto.md)|  | |

### Return type

[**EntitlementDetailResponseDto**](EntitlementDetailResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

