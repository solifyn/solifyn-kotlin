# RefundRequestsApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**refundRequestsList**](RefundRequestsApi.md#refundRequestsList) | **GET** /v1/refund-requests | List Refund Requests (Merchant) |
| [**refundRequestsListMessages**](RefundRequestsApi.md#refundRequestsListMessages) | **GET** /v1/refund-requests/{id}/messages | List Messages for Refund Request (Merchant) |
| [**refundRequestsSendMessage**](RefundRequestsApi.md#refundRequestsSendMessage) | **POST** /v1/refund-requests/{id}/messages | Send Refund Request Message (Merchant) |
| [**refundRequestsUpdateStatus**](RefundRequestsApi.md#refundRequestsUpdateStatus) | **PATCH** /v1/refund-requests/{id}/status | Update Refund Request Status (Merchant) |
| [**refundRequestsUploadEvidence**](RefundRequestsApi.md#refundRequestsUploadEvidence) | **POST** /v1/refund-requests/upload-evidence | Upload Dispute Evidence File (Merchant) |


<a id="refundRequestsList"></a>
# **refundRequestsList**
> refundRequestsList()

List Refund Requests (Merchant)

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = RefundRequestsApi()
try {
    apiInstance.refundRequestsList()
} catch (e: ClientException) {
    println("4xx response calling RefundRequestsApi#refundRequestsList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RefundRequestsApi#refundRequestsList")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="refundRequestsListMessages"></a>
# **refundRequestsListMessages**
> refundRequestsListMessages(id)

List Messages for Refund Request (Merchant)

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = RefundRequestsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.refundRequestsListMessages(id)
} catch (e: ClientException) {
    println("4xx response calling RefundRequestsApi#refundRequestsListMessages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RefundRequestsApi#refundRequestsListMessages")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="refundRequestsSendMessage"></a>
# **refundRequestsSendMessage**
> refundRequestsSendMessage(id)

Send Refund Request Message (Merchant)

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = RefundRequestsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.refundRequestsSendMessage(id)
} catch (e: ClientException) {
    println("4xx response calling RefundRequestsApi#refundRequestsSendMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RefundRequestsApi#refundRequestsSendMessage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="refundRequestsUpdateStatus"></a>
# **refundRequestsUpdateStatus**
> refundRequestsUpdateStatus(id)

Update Refund Request Status (Merchant)

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = RefundRequestsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.refundRequestsUpdateStatus(id)
} catch (e: ClientException) {
    println("4xx response calling RefundRequestsApi#refundRequestsUpdateStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RefundRequestsApi#refundRequestsUpdateStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="refundRequestsUploadEvidence"></a>
# **refundRequestsUploadEvidence**
> refundRequestsUploadEvidence()

Upload Dispute Evidence File (Merchant)

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = RefundRequestsApi()
try {
    apiInstance.refundRequestsUploadEvidence()
} catch (e: ClientException) {
    println("4xx response calling RefundRequestsApi#refundRequestsUploadEvidence")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RefundRequestsApi#refundRequestsUploadEvidence")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

