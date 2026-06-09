# WebhookApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**webhookControllerHandleSvixWebhook**](WebhookApi.md#webhookControllerHandleSvixWebhook) | **POST** /v1/webhook/svix |  |
| [**webhookControllerHandleWebhook**](WebhookApi.md#webhookControllerHandleWebhook) | **POST** /v1/webhook |  |


<a id="webhookControllerHandleSvixWebhook"></a>
# **webhookControllerHandleSvixWebhook**
> webhookControllerHandleSvixWebhook()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookApi()
try {
    apiInstance.webhookControllerHandleSvixWebhook()
} catch (e: ClientException) {
    println("4xx response calling WebhookApi#webhookControllerHandleSvixWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookApi#webhookControllerHandleSvixWebhook")
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

<a id="webhookControllerHandleWebhook"></a>
# **webhookControllerHandleWebhook**
> webhookControllerHandleWebhook(businessId)



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookApi()
val businessId : kotlin.String = businessId_example // kotlin.String | 
try {
    apiInstance.webhookControllerHandleWebhook(businessId)
} catch (e: ClientException) {
    println("4xx response calling WebhookApi#webhookControllerHandleWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookApi#webhookControllerHandleWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **businessId** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

