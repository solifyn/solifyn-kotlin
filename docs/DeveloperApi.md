# DeveloperApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**developerControllerCreateApiKey**](DeveloperApi.md#developerControllerCreateApiKey) | **POST** /v1/developer/api-keys |  |
| [**developerControllerCreateWebhookEndpoint**](DeveloperApi.md#developerControllerCreateWebhookEndpoint) | **POST** /v1/developer/webhooks |  |
| [**developerControllerDeleteApiKey**](DeveloperApi.md#developerControllerDeleteApiKey) | **DELETE** /v1/developer/api-keys/{id} |  |
| [**developerControllerDeleteWebhookEndpoint**](DeveloperApi.md#developerControllerDeleteWebhookEndpoint) | **DELETE** /v1/developer/webhooks/{id} |  |
| [**developerControllerGetApiKeys**](DeveloperApi.md#developerControllerGetApiKeys) | **GET** /v1/developer/api-keys |  |
| [**developerControllerGetAppPortalUrl**](DeveloperApi.md#developerControllerGetAppPortalUrl) | **GET** /v1/developer/webhooks/app-portal |  |
| [**developerControllerGetWebhookDeliveries**](DeveloperApi.md#developerControllerGetWebhookDeliveries) | **GET** /v1/developer/webhooks/{id}/deliveries |  |
| [**developerControllerGetWebhookEndpoints**](DeveloperApi.md#developerControllerGetWebhookEndpoints) | **GET** /v1/developer/webhooks |  |
| [**developerControllerUpdateWebhookEndpoint**](DeveloperApi.md#developerControllerUpdateWebhookEndpoint) | **PATCH** /v1/developer/webhooks/{id} |  |


<a id="developerControllerCreateApiKey"></a>
# **developerControllerCreateApiKey**
> developerControllerCreateApiKey()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
try {
    apiInstance.developerControllerCreateApiKey()
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerControllerCreateApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerControllerCreateApiKey")
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

<a id="developerControllerCreateWebhookEndpoint"></a>
# **developerControllerCreateWebhookEndpoint**
> developerControllerCreateWebhookEndpoint()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
try {
    apiInstance.developerControllerCreateWebhookEndpoint()
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerControllerCreateWebhookEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerControllerCreateWebhookEndpoint")
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

<a id="developerControllerDeleteApiKey"></a>
# **developerControllerDeleteApiKey**
> developerControllerDeleteApiKey(id)



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.developerControllerDeleteApiKey(id)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerControllerDeleteApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerControllerDeleteApiKey")
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

<a id="developerControllerDeleteWebhookEndpoint"></a>
# **developerControllerDeleteWebhookEndpoint**
> developerControllerDeleteWebhookEndpoint(id)



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.developerControllerDeleteWebhookEndpoint(id)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerControllerDeleteWebhookEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerControllerDeleteWebhookEndpoint")
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

<a id="developerControllerGetApiKeys"></a>
# **developerControllerGetApiKeys**
> developerControllerGetApiKeys()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
try {
    apiInstance.developerControllerGetApiKeys()
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerControllerGetApiKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerControllerGetApiKeys")
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

<a id="developerControllerGetAppPortalUrl"></a>
# **developerControllerGetAppPortalUrl**
> developerControllerGetAppPortalUrl()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
try {
    apiInstance.developerControllerGetAppPortalUrl()
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerControllerGetAppPortalUrl")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerControllerGetAppPortalUrl")
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

<a id="developerControllerGetWebhookDeliveries"></a>
# **developerControllerGetWebhookDeliveries**
> developerControllerGetWebhookDeliveries(id)



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.developerControllerGetWebhookDeliveries(id)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerControllerGetWebhookDeliveries")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerControllerGetWebhookDeliveries")
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

<a id="developerControllerGetWebhookEndpoints"></a>
# **developerControllerGetWebhookEndpoints**
> developerControllerGetWebhookEndpoints()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
try {
    apiInstance.developerControllerGetWebhookEndpoints()
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerControllerGetWebhookEndpoints")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerControllerGetWebhookEndpoints")
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

<a id="developerControllerUpdateWebhookEndpoint"></a>
# **developerControllerUpdateWebhookEndpoint**
> developerControllerUpdateWebhookEndpoint(id)



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.developerControllerUpdateWebhookEndpoint(id)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerControllerUpdateWebhookEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerControllerUpdateWebhookEndpoint")
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

