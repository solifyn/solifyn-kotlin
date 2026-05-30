# DigitalFileApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**digitalFileControllerCreate**](DigitalFileApi.md#digitalFileControllerCreate) | **POST** /v1/digital-files |  |
| [**digitalFileControllerFindAll**](DigitalFileApi.md#digitalFileControllerFindAll) | **GET** /v1/digital-files |  |
| [**digitalFileControllerRemove**](DigitalFileApi.md#digitalFileControllerRemove) | **DELETE** /v1/digital-files/{id} |  |


<a id="digitalFileControllerCreate"></a>
# **digitalFileControllerCreate**
> digitalFileControllerCreate()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DigitalFileApi()
try {
    apiInstance.digitalFileControllerCreate()
} catch (e: ClientException) {
    println("4xx response calling DigitalFileApi#digitalFileControllerCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DigitalFileApi#digitalFileControllerCreate")
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

<a id="digitalFileControllerFindAll"></a>
# **digitalFileControllerFindAll**
> digitalFileControllerFindAll()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DigitalFileApi()
try {
    apiInstance.digitalFileControllerFindAll()
} catch (e: ClientException) {
    println("4xx response calling DigitalFileApi#digitalFileControllerFindAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DigitalFileApi#digitalFileControllerFindAll")
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

<a id="digitalFileControllerRemove"></a>
# **digitalFileControllerRemove**
> digitalFileControllerRemove(id)



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DigitalFileApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.digitalFileControllerRemove(id)
} catch (e: ClientException) {
    println("4xx response calling DigitalFileApi#digitalFileControllerRemove")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DigitalFileApi#digitalFileControllerRemove")
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

