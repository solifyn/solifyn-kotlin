# LicenseKeysClientApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**licensesActivate**](LicenseKeysClientApi.md#licensesActivate) | **POST** /v1/licenses/activate | Activate License Key |
| [**licensesDeactivate**](LicenseKeysClientApi.md#licensesDeactivate) | **POST** /v1/licenses/deactivate/{instanceId} | Deactivate Instance |
| [**licensesInstances**](LicenseKeysClientApi.md#licensesInstances) | **GET** /v1/licenses/instances/{licenseId} | Get Active Instances |
| [**licensesVerify**](LicenseKeysClientApi.md#licensesVerify) | **POST** /v1/licenses/verify | Validate License Key |


<a id="licensesActivate"></a>
# **licensesActivate**
> Instance licensesActivate(licensesActivateRequest)

Activate License Key

Register and activate a device or instance for a specific license key.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseKeysClientApi()
val licensesActivateRequest : LicensesActivateRequest =  // LicensesActivateRequest | 
try {
    val result : Instance = apiInstance.licensesActivate(licensesActivateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseKeysClientApi#licensesActivate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseKeysClientApi#licensesActivate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **licensesActivateRequest** | [**LicensesActivateRequest**](LicensesActivateRequest.md)|  | |

### Return type

[**Instance**](Instance.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="licensesDeactivate"></a>
# **licensesDeactivate**
> LicensesDeactivate200Response licensesDeactivate(instanceId, licensesDeactivateRequest)

Deactivate Instance

Deactivate or unregister an active device instance from a license key.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseKeysClientApi()
val instanceId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | The unique device instance ID.
val licensesDeactivateRequest : LicensesDeactivateRequest =  // LicensesDeactivateRequest | 
try {
    val result : LicensesDeactivate200Response = apiInstance.licensesDeactivate(instanceId, licensesDeactivateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseKeysClientApi#licensesDeactivate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseKeysClientApi#licensesDeactivate")
    e.printStackTrace()
}
```

### Parameters
| **instanceId** | **java.util.UUID**| The unique device instance ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **licensesDeactivateRequest** | [**LicensesDeactivateRequest**](LicensesDeactivateRequest.md)|  | |

### Return type

[**LicensesDeactivate200Response**](LicensesDeactivate200Response.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="licensesInstances"></a>
# **licensesInstances**
> kotlin.collections.List&lt;Instance&gt; licensesInstances(licenseId)

Get Active Instances

List all active devices or server instances linked to a specific license key.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseKeysClientApi()
val licenseId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | The unique license key ID.
try {
    val result : kotlin.collections.List<Instance> = apiInstance.licensesInstances(licenseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseKeysClientApi#licensesInstances")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseKeysClientApi#licensesInstances")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **licenseId** | **java.util.UUID**| The unique license key ID. | |

### Return type

[**kotlin.collections.List&lt;Instance&gt;**](Instance.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="licensesVerify"></a>
# **licensesVerify**
> LicenseValidationResponse licensesVerify(licensesVerifyRequest)

Validate License Key

Verify if a software license key is valid, active, and has not exceeded its limits.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = LicenseKeysClientApi()
val licensesVerifyRequest : LicensesVerifyRequest =  // LicensesVerifyRequest | 
try {
    val result : LicenseValidationResponse = apiInstance.licensesVerify(licensesVerifyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LicenseKeysClientApi#licensesVerify")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LicenseKeysClientApi#licensesVerify")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **licensesVerifyRequest** | [**LicensesVerifyRequest**](LicensesVerifyRequest.md)|  | |

### Return type

[**LicenseValidationResponse**](LicenseValidationResponse.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

