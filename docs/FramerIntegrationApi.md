# FramerIntegrationApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**framerCreateTemplate**](FramerIntegrationApi.md#framerCreateTemplate) | **POST** /v1/framer/templates | Create Framer Template |
| [**framerDeleteTemplate**](FramerIntegrationApi.md#framerDeleteTemplate) | **DELETE** /v1/framer/templates/{id} | Delete Framer Template |
| [**framerGetTemplate**](FramerIntegrationApi.md#framerGetTemplate) | **GET** /v1/framer/templates/{id} | Retrieve Framer Template |
| [**framerListTemplates**](FramerIntegrationApi.md#framerListTemplates) | **GET** /v1/framer/templates | List Framer Templates |
| [**framerUpdateTemplate**](FramerIntegrationApi.md#framerUpdateTemplate) | **PUT** /v1/framer/templates/{id} | Update Framer Template |


<a id="framerCreateTemplate"></a>
# **framerCreateTemplate**
> FramerTemplateResponseDto framerCreateTemplate(createFramerTemplateDto)

Create Framer Template

Registers a new Framer template with its public remix link for the active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = FramerIntegrationApi()
val createFramerTemplateDto : CreateFramerTemplateDto =  // CreateFramerTemplateDto | 
try {
    val result : FramerTemplateResponseDto = apiInstance.framerCreateTemplate(createFramerTemplateDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FramerIntegrationApi#framerCreateTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FramerIntegrationApi#framerCreateTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createFramerTemplateDto** | [**CreateFramerTemplateDto**](CreateFramerTemplateDto.md)|  | |

### Return type

[**FramerTemplateResponseDto**](FramerTemplateResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="framerDeleteTemplate"></a>
# **framerDeleteTemplate**
> framerDeleteTemplate(id)

Delete Framer Template

Deletes a registered Framer template for the active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = FramerIntegrationApi()
val id : kotlin.String = id_example // kotlin.String | The Framer template ID
try {
    apiInstance.framerDeleteTemplate(id)
} catch (e: ClientException) {
    println("4xx response calling FramerIntegrationApi#framerDeleteTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FramerIntegrationApi#framerDeleteTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The Framer template ID | |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="framerGetTemplate"></a>
# **framerGetTemplate**
> FramerTemplateResponseDto framerGetTemplate(id)

Retrieve Framer Template

Retrieves details of a specific registered Framer template.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = FramerIntegrationApi()
val id : kotlin.String = id_example // kotlin.String | The Framer template ID
try {
    val result : FramerTemplateResponseDto = apiInstance.framerGetTemplate(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FramerIntegrationApi#framerGetTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FramerIntegrationApi#framerGetTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The Framer template ID | |

### Return type

[**FramerTemplateResponseDto**](FramerTemplateResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="framerListTemplates"></a>
# **framerListTemplates**
> kotlin.collections.List&lt;FramerTemplateResponseDto&gt; framerListTemplates()

List Framer Templates

Retrieves all registered Framer templates for the active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = FramerIntegrationApi()
try {
    val result : kotlin.collections.List<FramerTemplateResponseDto> = apiInstance.framerListTemplates()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FramerIntegrationApi#framerListTemplates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FramerIntegrationApi#framerListTemplates")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;FramerTemplateResponseDto&gt;**](FramerTemplateResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="framerUpdateTemplate"></a>
# **framerUpdateTemplate**
> FramerTemplateResponseDto framerUpdateTemplate(id, updateFramerTemplateDto)

Update Framer Template

Updates a registered Framer template for the active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = FramerIntegrationApi()
val id : kotlin.String = id_example // kotlin.String | The Framer template ID
val updateFramerTemplateDto : UpdateFramerTemplateDto =  // UpdateFramerTemplateDto | 
try {
    val result : FramerTemplateResponseDto = apiInstance.framerUpdateTemplate(id, updateFramerTemplateDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FramerIntegrationApi#framerUpdateTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FramerIntegrationApi#framerUpdateTemplate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The Framer template ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateFramerTemplateDto** | [**UpdateFramerTemplateDto**](UpdateFramerTemplateDto.md)|  | |

### Return type

[**FramerTemplateResponseDto**](FramerTemplateResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

