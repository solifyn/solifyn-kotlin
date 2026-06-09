# DeveloperApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**developerCreateApiKey**](DeveloperApi.md#developerCreateApiKey) | **POST** /v1/developer/api-keys | Create Developer API Key |
| [**developerCreateWebhook**](DeveloperApi.md#developerCreateWebhook) | **POST** /v1/developer/webhooks | Create Webhook Endpoint |
| [**developerDeleteWebhook**](DeveloperApi.md#developerDeleteWebhook) | **DELETE** /v1/developer/webhooks/{id} | Delete Webhook Endpoint |
| [**developerGetAppPortal**](DeveloperApi.md#developerGetAppPortal) | **GET** /v1/developer/webhooks/app-portal | Retrieve Hosted Webhooks Portal URL |
| [**developerGetWebhook**](DeveloperApi.md#developerGetWebhook) | **GET** /v1/developer/webhooks/{id} | Retrieve Webhook Endpoint Details |
| [**developerListApiKeys**](DeveloperApi.md#developerListApiKeys) | **GET** /v1/developer/api-keys | List Developer API Keys |
| [**developerListWebhookDeliveries**](DeveloperApi.md#developerListWebhookDeliveries) | **GET** /v1/developer/webhooks/{id}/deliveries | Retrieve Webhook Delivery Logs |
| [**developerListWebhooks**](DeveloperApi.md#developerListWebhooks) | **GET** /v1/developer/webhooks | List Webhook Endpoints |
| [**developerRevokeApiKey**](DeveloperApi.md#developerRevokeApiKey) | **DELETE** /v1/developer/api-keys/{id} | Revoke API Key |
| [**developerUpdateWebhook**](DeveloperApi.md#developerUpdateWebhook) | **PATCH** /v1/developer/webhooks/{id} | Update Webhook Endpoint |


<a id="developerCreateApiKey"></a>
# **developerCreateApiKey**
> ApiKeyResponseDto developerCreateApiKey(createApiKeyDto)

Create Developer API Key

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val createApiKeyDto : CreateApiKeyDto =  // CreateApiKeyDto | 
try {
    val result : ApiKeyResponseDto = apiInstance.developerCreateApiKey(createApiKeyDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerCreateApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerCreateApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createApiKeyDto** | [**CreateApiKeyDto**](CreateApiKeyDto.md)|  | |

### Return type

[**ApiKeyResponseDto**](ApiKeyResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="developerCreateWebhook"></a>
# **developerCreateWebhook**
> WebhookEndpointResponseDto developerCreateWebhook(createWebhookEndpointDto)

Create Webhook Endpoint

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val createWebhookEndpointDto : CreateWebhookEndpointDto =  // CreateWebhookEndpointDto | 
try {
    val result : WebhookEndpointResponseDto = apiInstance.developerCreateWebhook(createWebhookEndpointDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerCreateWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerCreateWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createWebhookEndpointDto** | [**CreateWebhookEndpointDto**](CreateWebhookEndpointDto.md)|  | |

### Return type

[**WebhookEndpointResponseDto**](WebhookEndpointResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="developerDeleteWebhook"></a>
# **developerDeleteWebhook**
> developerDeleteWebhook(id)

Delete Webhook Endpoint

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val id : kotlin.String = id_example // kotlin.String | The webhook endpoint ID
try {
    apiInstance.developerDeleteWebhook(id)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerDeleteWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerDeleteWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The webhook endpoint ID | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="developerGetAppPortal"></a>
# **developerGetAppPortal**
> AppPortalUrlResponseDto developerGetAppPortal()

Retrieve Hosted Webhooks Portal URL

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
try {
    val result : AppPortalUrlResponseDto = apiInstance.developerGetAppPortal()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerGetAppPortal")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerGetAppPortal")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AppPortalUrlResponseDto**](AppPortalUrlResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="developerGetWebhook"></a>
# **developerGetWebhook**
> WebhookEndpointResponseDto developerGetWebhook(id)

Retrieve Webhook Endpoint Details

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val id : kotlin.String = id_example // kotlin.String | The webhook endpoint ID
try {
    val result : WebhookEndpointResponseDto = apiInstance.developerGetWebhook(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerGetWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerGetWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The webhook endpoint ID | |

### Return type

[**WebhookEndpointResponseDto**](WebhookEndpointResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="developerListApiKeys"></a>
# **developerListApiKeys**
> kotlin.collections.List&lt;ApiKeyResponseDto&gt; developerListApiKeys()

List Developer API Keys

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
try {
    val result : kotlin.collections.List<ApiKeyResponseDto> = apiInstance.developerListApiKeys()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerListApiKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerListApiKeys")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ApiKeyResponseDto&gt;**](ApiKeyResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="developerListWebhookDeliveries"></a>
# **developerListWebhookDeliveries**
> kotlin.collections.List&lt;WebhookDeliveryResponseDto&gt; developerListWebhookDeliveries(id)

Retrieve Webhook Delivery Logs

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val id : kotlin.String = id_example // kotlin.String | The webhook endpoint ID
try {
    val result : kotlin.collections.List<WebhookDeliveryResponseDto> = apiInstance.developerListWebhookDeliveries(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerListWebhookDeliveries")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerListWebhookDeliveries")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The webhook endpoint ID | |

### Return type

[**kotlin.collections.List&lt;WebhookDeliveryResponseDto&gt;**](WebhookDeliveryResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="developerListWebhooks"></a>
# **developerListWebhooks**
> kotlin.collections.List&lt;WebhookEndpointResponseDto&gt; developerListWebhooks()

List Webhook Endpoints

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
try {
    val result : kotlin.collections.List<WebhookEndpointResponseDto> = apiInstance.developerListWebhooks()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerListWebhooks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerListWebhooks")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;WebhookEndpointResponseDto&gt;**](WebhookEndpointResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="developerRevokeApiKey"></a>
# **developerRevokeApiKey**
> developerRevokeApiKey(id)

Revoke API Key

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val id : kotlin.String = id_example // kotlin.String | The API key ID
try {
    apiInstance.developerRevokeApiKey(id)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerRevokeApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerRevokeApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The API key ID | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="developerUpdateWebhook"></a>
# **developerUpdateWebhook**
> WebhookEndpointResponseDto developerUpdateWebhook(id, updateWebhookEndpointDto)

Update Webhook Endpoint

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DeveloperApi()
val id : kotlin.String = id_example // kotlin.String | The webhook endpoint ID
val updateWebhookEndpointDto : UpdateWebhookEndpointDto =  // UpdateWebhookEndpointDto | 
try {
    val result : WebhookEndpointResponseDto = apiInstance.developerUpdateWebhook(id, updateWebhookEndpointDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeveloperApi#developerUpdateWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeveloperApi#developerUpdateWebhook")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The webhook endpoint ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateWebhookEndpointDto** | [**UpdateWebhookEndpointDto**](UpdateWebhookEndpointDto.md)|  | |

### Return type

[**WebhookEndpointResponseDto**](WebhookEndpointResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

