# MetersApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**eventsIngest**](MetersApi.md#eventsIngest) | **POST** /v1/meters/ingest | Ingest Events |
| [**metersCreate**](MetersApi.md#metersCreate) | **POST** /v1/meters | Create Meter |
| [**metersGet**](MetersApi.md#metersGet) | **GET** /v1/meters/{id} | Retrieve Meter |
| [**metersGetEvents**](MetersApi.md#metersGetEvents) | **GET** /v1/meters/{id}/events | List Meter Events |
| [**metersGetQuantities**](MetersApi.md#metersGetQuantities) | **GET** /v1/meters/{id}/quantities | Get Meter Quantities |
| [**metersList**](MetersApi.md#metersList) | **GET** /v1/meters | List Meters |
| [**metersUpdate**](MetersApi.md#metersUpdate) | **PATCH** /v1/meters/{id} | Update Meter |


<a id="eventsIngest"></a>
# **eventsIngest**
> MeterIngestResponseDto eventsIngest(meterIngestRequestDto)

Ingest Events

Ingest usage events for meters.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = MetersApi()
val meterIngestRequestDto : MeterIngestRequestDto =  // MeterIngestRequestDto | 
try {
    val result : MeterIngestResponseDto = apiInstance.eventsIngest(meterIngestRequestDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetersApi#eventsIngest")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetersApi#eventsIngest")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **meterIngestRequestDto** | [**MeterIngestRequestDto**](MeterIngestRequestDto.md)|  | |

### Return type

[**MeterIngestResponseDto**](MeterIngestResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="metersCreate"></a>
# **metersCreate**
> MeterResponseDto metersCreate(createMeterDto)

Create Meter

Create a new usage meter for event-based billing and usage tracking.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = MetersApi()
val createMeterDto : CreateMeterDto =  // CreateMeterDto | 
try {
    val result : MeterResponseDto = apiInstance.metersCreate(createMeterDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetersApi#metersCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetersApi#metersCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createMeterDto** | [**CreateMeterDto**](CreateMeterDto.md)|  | |

### Return type

[**MeterResponseDto**](MeterResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="metersGet"></a>
# **metersGet**
> MeterDetailResponseDto metersGet(id, startDate, endDate)

Retrieve Meter

Retrieve a meter and its most recent usage events.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = MetersApi()
val id : kotlin.String = mtr_8Z1aB2cD3eF4gH5iJ6kL7m // kotlin.String | The unique meter ID.
val startDate : kotlin.String = startDate_example // kotlin.String | 
val endDate : kotlin.String = endDate_example // kotlin.String | 
try {
    val result : MeterDetailResponseDto = apiInstance.metersGet(id, startDate, endDate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetersApi#metersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetersApi#metersGet")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique meter ID. | |
| **startDate** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endDate** | **kotlin.String**|  | |

### Return type

[**MeterDetailResponseDto**](MeterDetailResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="metersGetEvents"></a>
# **metersGetEvents**
> MeterEventsResponseDto metersGetEvents(id, limit)

List Meter Events

List recent usage events recorded for a meter.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = MetersApi()
val id : kotlin.String = mtr_8Z1aB2cD3eF4gH5iJ6kL7m // kotlin.String | The unique meter ID.
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Maximum number of usage events to return.
try {
    val result : MeterEventsResponseDto = apiInstance.metersGetEvents(id, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetersApi#metersGetEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetersApi#metersGetEvents")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique meter ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **java.math.BigDecimal**| Maximum number of usage events to return. | [optional] [default to 100] |

### Return type

[**MeterEventsResponseDto**](MeterEventsResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="metersGetQuantities"></a>
# **metersGetQuantities**
> MeterQuantitiesResponseDto metersGetQuantities(id, startDate, endDate)

Get Meter Quantities

Get aggregated usage quantities for a meter within an optional date range.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = MetersApi()
val id : kotlin.String = mtr_8Z1aB2cD3eF4gH5iJ6kL7m // kotlin.String | The unique meter ID.
val startDate : kotlin.String = startDate_example // kotlin.String | Inclusive start date in ISO 8601 format.
val endDate : kotlin.String = endDate_example // kotlin.String | Inclusive end date in ISO 8601 format.
try {
    val result : MeterQuantitiesResponseDto = apiInstance.metersGetQuantities(id, startDate, endDate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetersApi#metersGetQuantities")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetersApi#metersGetQuantities")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique meter ID. | |
| **startDate** | **kotlin.String**| Inclusive start date in ISO 8601 format. | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endDate** | **kotlin.String**| Inclusive end date in ISO 8601 format. | [optional] |

### Return type

[**MeterQuantitiesResponseDto**](MeterQuantitiesResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="metersList"></a>
# **metersList**
> kotlin.collections.List&lt;MeterResponseDto&gt; metersList(status)

List Meters

List meters belonging to your active business. You can filter by archived status.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = MetersApi()
val status : kotlin.String = status_example // kotlin.String | Filter by meter status.
try {
    val result : kotlin.collections.List<MeterResponseDto> = apiInstance.metersList(status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetersApi#metersList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetersApi#metersList")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**| Filter by meter status. | [optional] [enum: active, archived] |

### Return type

[**kotlin.collections.List&lt;MeterResponseDto&gt;**](MeterResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="metersUpdate"></a>
# **metersUpdate**
> MeterResponseDto metersUpdate(id, updateMeterDto)

Update Meter

Update an existing meter definition.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = MetersApi()
val id : kotlin.String = mtr_8Z1aB2cD3eF4gH5iJ6kL7m // kotlin.String | The unique meter ID.
val updateMeterDto : UpdateMeterDto =  // UpdateMeterDto | 
try {
    val result : MeterResponseDto = apiInstance.metersUpdate(id, updateMeterDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetersApi#metersUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetersApi#metersUpdate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique meter ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateMeterDto** | [**UpdateMeterDto**](UpdateMeterDto.md)|  | |

### Return type

[**MeterResponseDto**](MeterResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

