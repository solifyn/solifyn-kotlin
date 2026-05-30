# BalanceApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**balanceControllerFindAll**](BalanceApi.md#balanceControllerFindAll) | **GET** /v1/balances |  |
| [**balanceControllerGenerateReport**](BalanceApi.md#balanceControllerGenerateReport) | **GET** /v1/balances/report |  |
| [**balanceControllerGetSummary**](BalanceApi.md#balanceControllerGetSummary) | **GET** /v1/balances/summary |  |


<a id="balanceControllerFindAll"></a>
# **balanceControllerFindAll**
> balanceControllerFindAll()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = BalanceApi()
try {
    apiInstance.balanceControllerFindAll()
} catch (e: ClientException) {
    println("4xx response calling BalanceApi#balanceControllerFindAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BalanceApi#balanceControllerFindAll")
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

<a id="balanceControllerGenerateReport"></a>
# **balanceControllerGenerateReport**
> balanceControllerGenerateReport()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = BalanceApi()
try {
    apiInstance.balanceControllerGenerateReport()
} catch (e: ClientException) {
    println("4xx response calling BalanceApi#balanceControllerGenerateReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BalanceApi#balanceControllerGenerateReport")
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

<a id="balanceControllerGetSummary"></a>
# **balanceControllerGetSummary**
> balanceControllerGetSummary()



### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = BalanceApi()
try {
    apiInstance.balanceControllerGetSummary()
} catch (e: ClientException) {
    println("4xx response calling BalanceApi#balanceControllerGetSummary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BalanceApi#balanceControllerGetSummary")
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

