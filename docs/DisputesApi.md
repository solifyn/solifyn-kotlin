# DisputesApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**disputesGenerateReport**](DisputesApi.md#disputesGenerateReport) | **GET** /v1/transactions/disputes/report | Generate Dispute CSV Report |
| [**disputesGet**](DisputesApi.md#disputesGet) | **GET** /v1/transactions/disputes/{id} | Retrieve Dispute |
| [**disputesList**](DisputesApi.md#disputesList) | **GET** /v1/transactions/disputes | List Disputes |
| [**disputesSubmitEvidence**](DisputesApi.md#disputesSubmitEvidence) | **POST** /v1/transactions/disputes/{id}/submit | Submit Dispute Evidence |
| [**disputesUpdateEvidence**](DisputesApi.md#disputesUpdateEvidence) | **PATCH** /v1/transactions/disputes/{id}/evidence | Update Dispute Evidence |
| [**disputesUploadEvidenceFile**](DisputesApi.md#disputesUploadEvidenceFile) | **POST** /v1/transactions/disputes/upload | Upload Evidence File |


<a id="disputesGenerateReport"></a>
# **disputesGenerateReport**
> disputesGenerateReport(createdAtGte, createdAtLte, status)

Generate Dispute CSV Report

Generates a downloadable CSV report of disputes matching the filters.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DisputesApi()
val createdAtGte : kotlin.String = createdAtGte_example // kotlin.String | Filter disputes created after this ISO date-time string
val createdAtLte : kotlin.String = createdAtLte_example // kotlin.String | Filter disputes created before this ISO date-time string
val status : kotlin.String = status_example // kotlin.String | Filter disputes by status
try {
    apiInstance.disputesGenerateReport(createdAtGte, createdAtLte, status)
} catch (e: ClientException) {
    println("4xx response calling DisputesApi#disputesGenerateReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DisputesApi#disputesGenerateReport")
    e.printStackTrace()
}
```

### Parameters
| **createdAtGte** | **kotlin.String**| Filter disputes created after this ISO date-time string | [optional] |
| **createdAtLte** | **kotlin.String**| Filter disputes created before this ISO date-time string | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**| Filter disputes by status | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="disputesGet"></a>
# **disputesGet**
> Dispute disputesGet(id)

Retrieve Dispute

Retrieve details of a specific dispute by ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DisputesApi()
val id : kotlin.String = dsp_123 // kotlin.String | The dispute ID
try {
    val result : Dispute = apiInstance.disputesGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DisputesApi#disputesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DisputesApi#disputesGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The dispute ID | |

### Return type

[**Dispute**](Dispute.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="disputesList"></a>
# **disputesList**
> DisputeList disputesList(page, limit, status, type)

List Disputes

Retrieve disputes associated with the active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DisputesApi()
val page : kotlin.String = 1 // kotlin.String | Page number for pagination
val limit : kotlin.String = 10 // kotlin.String | Page size limit for pagination
val status : kotlin.String = status_example // kotlin.String | Filter disputes by status
val type : kotlin.String = type_example // kotlin.String | Filter by type: dispute or alert
try {
    val result : DisputeList = apiInstance.disputesList(page, limit, status, type)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DisputesApi#disputesList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DisputesApi#disputesList")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.String**| Page number for pagination | [optional] |
| **limit** | **kotlin.String**| Page size limit for pagination | [optional] |
| **status** | **kotlin.String**| Filter disputes by status | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **type** | **kotlin.String**| Filter by type: dispute or alert | [optional] |

### Return type

[**DisputeList**](DisputeList.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="disputesSubmitEvidence"></a>
# **disputesSubmitEvidence**
> Dispute disputesSubmitEvidence(id)

Submit Dispute Evidence

Finalize and submit the uploaded evidence for review.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DisputesApi()
val id : kotlin.String = dsp_123 // kotlin.String | The dispute ID
try {
    val result : Dispute = apiInstance.disputesSubmitEvidence(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DisputesApi#disputesSubmitEvidence")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DisputesApi#disputesSubmitEvidence")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The dispute ID | |

### Return type

[**Dispute**](Dispute.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="disputesUpdateEvidence"></a>
# **disputesUpdateEvidence**
> Dispute disputesUpdateEvidence(id, disputeEvidenceUpdate)

Update Dispute Evidence

Upload and update evidence attachments for a dispute.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DisputesApi()
val id : kotlin.String = dsp_123 // kotlin.String | The dispute ID
val disputeEvidenceUpdate : DisputeEvidenceUpdate =  // DisputeEvidenceUpdate | 
try {
    val result : Dispute = apiInstance.disputesUpdateEvidence(id, disputeEvidenceUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DisputesApi#disputesUpdateEvidence")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DisputesApi#disputesUpdateEvidence")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The dispute ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **disputeEvidenceUpdate** | [**DisputeEvidenceUpdate**](DisputeEvidenceUpdate.md)|  | |

### Return type

[**Dispute**](Dispute.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="disputesUploadEvidenceFile"></a>
# **disputesUploadEvidenceFile**
> DisputeFileUpload disputesUploadEvidenceFile(file)

Upload Evidence File

Upload a support file (image, PDF, video) to use as dispute evidence.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DisputesApi()
val file : java.io.File = BINARY_DATA_HERE // java.io.File | The evidence file to upload (Max 25MB: JPEG, PNG, GIF, WEBP, PDF, MP4, WEBM, QuickTime)
try {
    val result : DisputeFileUpload = apiInstance.disputesUploadEvidenceFile(file)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DisputesApi#disputesUploadEvidenceFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DisputesApi#disputesUploadEvidenceFile")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file** | **java.io.File**| The evidence file to upload (Max 25MB: JPEG, PNG, GIF, WEBP, PDF, MP4, WEBM, QuickTime) | |

### Return type

[**DisputeFileUpload**](DisputeFileUpload.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

