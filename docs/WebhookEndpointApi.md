# WebhookEndpointApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**operationalWebhookControllerCreate**](WebhookEndpointApi.md#operationalWebhookControllerCreate) | **POST** /v1/operational-webhook/endpoint | Create Operational Webhook Endpoint |
| [**operationalWebhookControllerDelete**](WebhookEndpointApi.md#operationalWebhookControllerDelete) | **DELETE** /v1/operational-webhook/endpoint/{id} | Delete Operational Webhook Endpoint |
| [**operationalWebhookControllerGet**](WebhookEndpointApi.md#operationalWebhookControllerGet) | **GET** /v1/operational-webhook/endpoint/{id} | Get Operational Webhook Endpoint |
| [**operationalWebhookControllerGetHeaders**](WebhookEndpointApi.md#operationalWebhookControllerGetHeaders) | **GET** /v1/operational-webhook/endpoint/{id}/headers | Get Operational Webhook Endpoint Headers |
| [**operationalWebhookControllerGetSecret**](WebhookEndpointApi.md#operationalWebhookControllerGetSecret) | **GET** /v1/operational-webhook/endpoint/{id}/secret | Get Operational Webhook Endpoint Secret |
| [**operationalWebhookControllerList**](WebhookEndpointApi.md#operationalWebhookControllerList) | **GET** /v1/operational-webhook/endpoint | List Operational Webhook Endpoints |
| [**operationalWebhookControllerRotateSecret**](WebhookEndpointApi.md#operationalWebhookControllerRotateSecret) | **POST** /v1/operational-webhook/endpoint/{id}/secret/rotate | Rotate Operational Webhook Endpoint Secret |
| [**operationalWebhookControllerUpdate**](WebhookEndpointApi.md#operationalWebhookControllerUpdate) | **PUT** /v1/operational-webhook/endpoint/{id} | Update Operational Webhook Endpoint |
| [**operationalWebhookControllerUpdateHeaders**](WebhookEndpointApi.md#operationalWebhookControllerUpdateHeaders) | **PUT** /v1/operational-webhook/endpoint/{id}/headers | Set Operational Webhook Endpoint Headers |


<a id="operationalWebhookControllerCreate"></a>
# **operationalWebhookControllerCreate**
> OperationalWebhookEndpointResponseDto operationalWebhookControllerCreate(operationalWebhookEndpointInDto)

Create Operational Webhook Endpoint

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookEndpointApi()
val operationalWebhookEndpointInDto : OperationalWebhookEndpointInDto =  // OperationalWebhookEndpointInDto | 
try {
    val result : OperationalWebhookEndpointResponseDto = apiInstance.operationalWebhookControllerCreate(operationalWebhookEndpointInDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhookEndpointApi#operationalWebhookControllerCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookEndpointApi#operationalWebhookControllerCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **operationalWebhookEndpointInDto** | [**OperationalWebhookEndpointInDto**](OperationalWebhookEndpointInDto.md)|  | |

### Return type

[**OperationalWebhookEndpointResponseDto**](OperationalWebhookEndpointResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="operationalWebhookControllerDelete"></a>
# **operationalWebhookControllerDelete**
> operationalWebhookControllerDelete(id)

Delete Operational Webhook Endpoint

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookEndpointApi()
val id : kotlin.String = id_example // kotlin.String | The endpoint ID or UID
try {
    apiInstance.operationalWebhookControllerDelete(id)
} catch (e: ClientException) {
    println("4xx response calling WebhookEndpointApi#operationalWebhookControllerDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookEndpointApi#operationalWebhookControllerDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The endpoint ID or UID | |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="operationalWebhookControllerGet"></a>
# **operationalWebhookControllerGet**
> OperationalWebhookEndpointResponseDto operationalWebhookControllerGet(id)

Get Operational Webhook Endpoint

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookEndpointApi()
val id : kotlin.String = id_example // kotlin.String | The endpoint ID or UID
try {
    val result : OperationalWebhookEndpointResponseDto = apiInstance.operationalWebhookControllerGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhookEndpointApi#operationalWebhookControllerGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookEndpointApi#operationalWebhookControllerGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The endpoint ID or UID | |

### Return type

[**OperationalWebhookEndpointResponseDto**](OperationalWebhookEndpointResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="operationalWebhookControllerGetHeaders"></a>
# **operationalWebhookControllerGetHeaders**
> OperationalWebhookEndpointHeadersResponseDto operationalWebhookControllerGetHeaders(id)

Get Operational Webhook Endpoint Headers

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookEndpointApi()
val id : kotlin.String = id_example // kotlin.String | The endpoint ID or UID
try {
    val result : OperationalWebhookEndpointHeadersResponseDto = apiInstance.operationalWebhookControllerGetHeaders(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhookEndpointApi#operationalWebhookControllerGetHeaders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookEndpointApi#operationalWebhookControllerGetHeaders")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The endpoint ID or UID | |

### Return type

[**OperationalWebhookEndpointHeadersResponseDto**](OperationalWebhookEndpointHeadersResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="operationalWebhookControllerGetSecret"></a>
# **operationalWebhookControllerGetSecret**
> OperationalWebhookEndpointSecretResponseDto operationalWebhookControllerGetSecret(id)

Get Operational Webhook Endpoint Secret

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookEndpointApi()
val id : kotlin.String = id_example // kotlin.String | The endpoint ID or UID
try {
    val result : OperationalWebhookEndpointSecretResponseDto = apiInstance.operationalWebhookControllerGetSecret(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhookEndpointApi#operationalWebhookControllerGetSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookEndpointApi#operationalWebhookControllerGetSecret")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The endpoint ID or UID | |

### Return type

[**OperationalWebhookEndpointSecretResponseDto**](OperationalWebhookEndpointSecretResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="operationalWebhookControllerList"></a>
# **operationalWebhookControllerList**
> OperationalWebhookEndpointListResponseDto operationalWebhookControllerList()

List Operational Webhook Endpoints

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookEndpointApi()
try {
    val result : OperationalWebhookEndpointListResponseDto = apiInstance.operationalWebhookControllerList()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhookEndpointApi#operationalWebhookControllerList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookEndpointApi#operationalWebhookControllerList")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**OperationalWebhookEndpointListResponseDto**](OperationalWebhookEndpointListResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="operationalWebhookControllerRotateSecret"></a>
# **operationalWebhookControllerRotateSecret**
> operationalWebhookControllerRotateSecret(id, operationalWebhookEndpointSecretInDto)

Rotate Operational Webhook Endpoint Secret

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookEndpointApi()
val id : kotlin.String = id_example // kotlin.String | The endpoint ID or UID
val operationalWebhookEndpointSecretInDto : OperationalWebhookEndpointSecretInDto =  // OperationalWebhookEndpointSecretInDto | 
try {
    apiInstance.operationalWebhookControllerRotateSecret(id, operationalWebhookEndpointSecretInDto)
} catch (e: ClientException) {
    println("4xx response calling WebhookEndpointApi#operationalWebhookControllerRotateSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookEndpointApi#operationalWebhookControllerRotateSecret")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The endpoint ID or UID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **operationalWebhookEndpointSecretInDto** | [**OperationalWebhookEndpointSecretInDto**](OperationalWebhookEndpointSecretInDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="operationalWebhookControllerUpdate"></a>
# **operationalWebhookControllerUpdate**
> OperationalWebhookEndpointResponseDto operationalWebhookControllerUpdate(id, operationalWebhookEndpointUpdateDto)

Update Operational Webhook Endpoint

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookEndpointApi()
val id : kotlin.String = id_example // kotlin.String | The endpoint ID or UID
val operationalWebhookEndpointUpdateDto : OperationalWebhookEndpointUpdateDto =  // OperationalWebhookEndpointUpdateDto | 
try {
    val result : OperationalWebhookEndpointResponseDto = apiInstance.operationalWebhookControllerUpdate(id, operationalWebhookEndpointUpdateDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhookEndpointApi#operationalWebhookControllerUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookEndpointApi#operationalWebhookControllerUpdate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The endpoint ID or UID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **operationalWebhookEndpointUpdateDto** | [**OperationalWebhookEndpointUpdateDto**](OperationalWebhookEndpointUpdateDto.md)|  | |

### Return type

[**OperationalWebhookEndpointResponseDto**](OperationalWebhookEndpointResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="operationalWebhookControllerUpdateHeaders"></a>
# **operationalWebhookControllerUpdateHeaders**
> operationalWebhookControllerUpdateHeaders(id, operationalWebhookEndpointHeadersInDto)

Set Operational Webhook Endpoint Headers

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = WebhookEndpointApi()
val id : kotlin.String = id_example // kotlin.String | The endpoint ID or UID
val operationalWebhookEndpointHeadersInDto : OperationalWebhookEndpointHeadersInDto =  // OperationalWebhookEndpointHeadersInDto | 
try {
    apiInstance.operationalWebhookControllerUpdateHeaders(id, operationalWebhookEndpointHeadersInDto)
} catch (e: ClientException) {
    println("4xx response calling WebhookEndpointApi#operationalWebhookControllerUpdateHeaders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhookEndpointApi#operationalWebhookControllerUpdateHeaders")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The endpoint ID or UID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **operationalWebhookEndpointHeadersInDto** | [**OperationalWebhookEndpointHeadersInDto**](OperationalWebhookEndpointHeadersInDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

