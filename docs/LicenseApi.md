# LicenseApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**licensesCreate**](LicenseApi.md#licensesCreate) | **POST** /v1/licenses | Create License Key |
| [**licensesDeleteInstance**](LicenseApi.md#licensesDeleteInstance) | **DELETE** /v1/licenses/instances/{instanceId} | Force Delete Instance |
| [**licensesGet**](LicenseApi.md#licensesGet) | **GET** /v1/licenses/{id} | Get License Key |
| [**licensesGetInstance**](LicenseApi.md#licensesGetInstance) | **GET** /v1/licenses/{id}/instances/{instanceId} | Get License Key Instance |
| [**licensesGetInstances**](LicenseApi.md#licensesGetInstances) | **GET** /v1/licenses/{id}/instances | Get License Key Instances |
| [**licensesList**](LicenseApi.md#licensesList) | **GET** /v1/licenses | List License Keys |
| [**licensesToggle**](LicenseApi.md#licensesToggle) | **POST** /v1/licenses/{id}/toggle | Toggle License Status |
| [**licensesUpdate**](LicenseApi.md#licensesUpdate) | **PATCH** /v1/licenses/{id} | Update License Key |
| [**licensesUpdateInstance**](LicenseApi.md#licensesUpdateInstance) | **PATCH** /v1/licenses/{id}/instances/{instanceId} | Update License Key Instance |
| [**licensesUpdateInstancePost**](LicenseApi.md#licensesUpdateInstancePost) | **POST** /v1/licenses/{id}/instances/{instanceId} | Update License Key Instance (POST) |


<a id="licensesCreate"></a>
# **licensesCreate**
> License licensesCreate(licensesCreateRequest)

Create License Key

Manually issue a new license key for a specific product.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseApi()
val licensesCreateRequest : LicensesCreateRequest =  // LicensesCreateRequest | 
try {
    val result : License = apiInstance.licensesCreate(licensesCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseApi#licensesCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseApi#licensesCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **licensesCreateRequest** | [**LicensesCreateRequest**](LicensesCreateRequest.md)|  | |

### Return type

[**License**](License.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="licensesDeleteInstance"></a>
# **licensesDeleteInstance**
> Instance licensesDeleteInstance(instanceId)

Force Delete Instance

Administrative endpoint to force-delete an instance globally by its database ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseApi()
val instanceId : kotlin.String = inc_123 // kotlin.String | The unique hardware activation instance ID.
try {
    val result : Instance = apiInstance.licensesDeleteInstance(instanceId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseApi#licensesDeleteInstance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseApi#licensesDeleteInstance")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **instanceId** | **kotlin.String**| The unique hardware activation instance ID. | |

### Return type

[**Instance**](Instance.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="licensesGet"></a>
# **licensesGet**
> License licensesGet(id)

Get License Key

Retrieve complete administrative details of a specific license key.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | The unique license key ID.
try {
    val result : License = apiInstance.licensesGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseApi#licensesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseApi#licensesGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**| The unique license key ID. | |

### Return type

[**License**](License.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="licensesGetInstance"></a>
# **licensesGetInstance**
> Instance licensesGetInstance(id, instanceId)

Get License Key Instance

Retrieve administrative details of a specific software license instance.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | The unique administrative identifier (ID) of the parent license key.
val instanceId : kotlin.String = inc_123 // kotlin.String | The client-generated instance ID (hardware hash) or the internal database ID of the instance.
try {
    val result : Instance = apiInstance.licensesGetInstance(id, instanceId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseApi#licensesGetInstance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseApi#licensesGetInstance")
    e.printStackTrace()
}
```

### Parameters
| **id** | **java.util.UUID**| The unique administrative identifier (ID) of the parent license key. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **instanceId** | **kotlin.String**| The client-generated instance ID (hardware hash) or the internal database ID of the instance. | |

### Return type

[**Instance**](Instance.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="licensesGetInstances"></a>
# **licensesGetInstances**
> kotlin.collections.List&lt;Instance&gt; licensesGetInstances(id)

Get License Key Instances

Retrieve all active devices/instances for a specific administrative license key.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseApi()
val id : kotlin.String = lic_123 // kotlin.String | The unique administrative identifier (ID) of the parent license key.
try {
    val result : kotlin.collections.List<Instance> = apiInstance.licensesGetInstances(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseApi#licensesGetInstances")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseApi#licensesGetInstances")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique administrative identifier (ID) of the parent license key. | |

### Return type

[**kotlin.collections.List&lt;Instance&gt;**](Instance.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="licensesList"></a>
# **licensesList**
> kotlin.collections.List&lt;License&gt; licensesList()

List License Keys

List all administrative license keys belonging to products under your active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseApi()
try {
    val result : kotlin.collections.List<License> = apiInstance.licensesList()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseApi#licensesList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseApi#licensesList")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;License&gt;**](License.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="licensesToggle"></a>
# **licensesToggle**
> License licensesToggle(id)

Toggle License Status

Toggle the status of a specific license key between ACTIVE and DISABLED.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseApi()
val id : kotlin.String = lic_123 // kotlin.String | The unique license key ID.
try {
    val result : License = apiInstance.licensesToggle(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseApi#licensesToggle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseApi#licensesToggle")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique license key ID. | |

### Return type

[**License**](License.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="licensesUpdate"></a>
# **licensesUpdate**
> License licensesUpdate(id, licensesUpdateRequest)

Update License Key

Update limits or status of an existing license key.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | The unique license key ID.
val licensesUpdateRequest : LicensesUpdateRequest =  // LicensesUpdateRequest | 
try {
    val result : License = apiInstance.licensesUpdate(id, licensesUpdateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseApi#licensesUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseApi#licensesUpdate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **java.util.UUID**| The unique license key ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **licensesUpdateRequest** | [**LicensesUpdateRequest**](LicensesUpdateRequest.md)|  | |

### Return type

[**License**](License.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="licensesUpdateInstance"></a>
# **licensesUpdateInstance**
> Instance licensesUpdateInstance(instanceId, id, licensesUpdateInstancePostRequest)

Update License Key Instance

Update administrative details (like friendly display name or custom IP) of an active license device instance.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseApi()
val instanceId : kotlin.String = inc_123 // kotlin.String | The client-generated instance ID (hardware hash) or the internal database ID of the instance.
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | The unique administrative identifier (ID) of the parent license key.
val licensesUpdateInstancePostRequest : LicensesUpdateInstancePostRequest =  // LicensesUpdateInstancePostRequest | 
try {
    val result : Instance = apiInstance.licensesUpdateInstance(instanceId, id, licensesUpdateInstancePostRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseApi#licensesUpdateInstance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseApi#licensesUpdateInstance")
    e.printStackTrace()
}
```

### Parameters
| **instanceId** | **kotlin.String**| The client-generated instance ID (hardware hash) or the internal database ID of the instance. | |
| **id** | **java.util.UUID**| The unique administrative identifier (ID) of the parent license key. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **licensesUpdateInstancePostRequest** | [**LicensesUpdateInstancePostRequest**](LicensesUpdateInstancePostRequest.md)|  | |

### Return type

[**Instance**](Instance.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="licensesUpdateInstancePost"></a>
# **licensesUpdateInstancePost**
> Instance licensesUpdateInstancePost(instanceId, id, licensesUpdateInstancePostRequest)

Update License Key Instance (POST)

Alternative POST endpoint to update administrative details (like friendly display name or custom IP) of an active license device instance.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseApi()
val instanceId : kotlin.String = inc_123 // kotlin.String | The client-generated instance ID (hardware hash) or the internal database ID of the instance.
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | The unique administrative identifier (ID) of the parent license key.
val licensesUpdateInstancePostRequest : LicensesUpdateInstancePostRequest =  // LicensesUpdateInstancePostRequest | 
try {
    val result : Instance = apiInstance.licensesUpdateInstancePost(instanceId, id, licensesUpdateInstancePostRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseApi#licensesUpdateInstancePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseApi#licensesUpdateInstancePost")
    e.printStackTrace()
}
```

### Parameters
| **instanceId** | **kotlin.String**| The client-generated instance ID (hardware hash) or the internal database ID of the instance. | |
| **id** | **java.util.UUID**| The unique administrative identifier (ID) of the parent license key. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **licensesUpdateInstancePostRequest** | [**LicensesUpdateInstancePostRequest**](LicensesUpdateInstancePostRequest.md)|  | |

### Return type

[**Instance**](Instance.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

