# EntitlementGrantsApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**entitlementGrantsGet**](EntitlementGrantsApi.md#entitlementGrantsGet) | **GET** /v1/entitlement-grants/{id} | Retrieve Entitlement Grant |
| [**entitlementGrantsList**](EntitlementGrantsApi.md#entitlementGrantsList) | **GET** /v1/entitlement-grants | List Entitlement Grants |
| [**entitlementGrantsRetry**](EntitlementGrantsApi.md#entitlementGrantsRetry) | **POST** /v1/entitlement-grants/{id}/retry | Retry Entitlement Grant Delivery |
| [**entitlementGrantsRevoke**](EntitlementGrantsApi.md#entitlementGrantsRevoke) | **POST** /v1/entitlement-grants/{id}/revoke | Manually Revoke Entitlement Grant |


<a id="entitlementGrantsGet"></a>
# **entitlementGrantsGet**
> EntitlementGrantResponseDto entitlementGrantsGet(id)

Retrieve Entitlement Grant

Retrieve details of a specific entitlement grant.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = EntitlementGrantsApi()
val id : kotlin.String = id_example // kotlin.String | The unique grant ID
try {
    val result : EntitlementGrantResponseDto = apiInstance.entitlementGrantsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EntitlementGrantsApi#entitlementGrantsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EntitlementGrantsApi#entitlementGrantsGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique grant ID | |

### Return type

[**EntitlementGrantResponseDto**](EntitlementGrantResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="entitlementGrantsList"></a>
# **entitlementGrantsList**
> kotlin.collections.List&lt;EntitlementGrantResponseDto&gt; entitlementGrantsList(status)

List Entitlement Grants

Retrieve all GitHub repository entitlement grants for the active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = EntitlementGrantsApi()
val status : kotlin.String = status_example // kotlin.String | Filter by status (PENDING, DELIVERED, FAILED, REVOKED)
try {
    val result : kotlin.collections.List<EntitlementGrantResponseDto> = apiInstance.entitlementGrantsList(status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EntitlementGrantsApi#entitlementGrantsList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EntitlementGrantsApi#entitlementGrantsList")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**| Filter by status (PENDING, DELIVERED, FAILED, REVOKED) | [optional] |

### Return type

[**kotlin.collections.List&lt;EntitlementGrantResponseDto&gt;**](EntitlementGrantResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="entitlementGrantsRetry"></a>
# **entitlementGrantsRetry**
> EntitlementGrantResponseDto entitlementGrantsRetry(id)

Retry Entitlement Grant Delivery

Attempts to re-invite the collaborator if GitHub username is already connected, or resets the OAuth URL redirect.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = EntitlementGrantsApi()
val id : kotlin.String = id_example // kotlin.String | The unique grant ID
try {
    val result : EntitlementGrantResponseDto = apiInstance.entitlementGrantsRetry(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EntitlementGrantsApi#entitlementGrantsRetry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EntitlementGrantsApi#entitlementGrantsRetry")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique grant ID | |

### Return type

[**EntitlementGrantResponseDto**](EntitlementGrantResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="entitlementGrantsRevoke"></a>
# **entitlementGrantsRevoke**
> EntitlementGrantResponseDto entitlementGrantsRevoke(id)

Manually Revoke Entitlement Grant

Manually remove the customer collaborator access from the repository and revoke the grant.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = EntitlementGrantsApi()
val id : kotlin.String = id_example // kotlin.String | The unique grant ID
try {
    val result : EntitlementGrantResponseDto = apiInstance.entitlementGrantsRevoke(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EntitlementGrantsApi#entitlementGrantsRevoke")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EntitlementGrantsApi#entitlementGrantsRevoke")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique grant ID | |

### Return type

[**EntitlementGrantResponseDto**](EntitlementGrantResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

