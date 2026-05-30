# PayoutsApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**payoutsCreateWithdrawal**](PayoutsApi.md#payoutsCreateWithdrawal) | **POST** /v1/payouts/withdrawals | Create Withdrawal |
| [**payoutsGetAccount**](PayoutsApi.md#payoutsGetAccount) | **GET** /v1/payouts/account | Retrieve Payout Account |
| [**payoutsGetAccountLink**](PayoutsApi.md#payoutsGetAccountLink) | **GET** /v1/payouts/account-link | Create Account Link |
| [**payoutsGetToken**](PayoutsApi.md#payoutsGetToken) | **GET** /v1/payouts/token | Generate Portal Access Token |
| [**payoutsGetWithdrawals**](PayoutsApi.md#payoutsGetWithdrawals) | **GET** /v1/payouts/withdrawals | Get Withdrawals List |
| [**payoutsListMethods**](PayoutsApi.md#payoutsListMethods) | **GET** /v1/payouts/methods | List Payout Methods |
| [**payoutsListVerifications**](PayoutsApi.md#payoutsListVerifications) | **GET** /v1/payouts/verifications | List Verifications |
| [**payoutsListWithdrawals**](PayoutsApi.md#payoutsListWithdrawals) | **GET** /v1/payouts | List Withdrawals |


<a id="payoutsCreateWithdrawal"></a>
# **payoutsCreateWithdrawal**
> Withdrawal payoutsCreateWithdrawal(withdrawalCreate)

Create Withdrawal

Initiate a balance withdrawal transfer request.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = PayoutsApi()
val withdrawalCreate : WithdrawalCreate =  // WithdrawalCreate | 
try {
    val result : Withdrawal = apiInstance.payoutsCreateWithdrawal(withdrawalCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayoutsApi#payoutsCreateWithdrawal")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayoutsApi#payoutsCreateWithdrawal")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **withdrawalCreate** | [**WithdrawalCreate**](WithdrawalCreate.md)|  | |

### Return type

[**Withdrawal**](Withdrawal.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="payoutsGetAccount"></a>
# **payoutsGetAccount**
> PayoutAccount payoutsGetAccount()

Retrieve Payout Account

Retrieve general status and information of onboarding payout accounts.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = PayoutsApi()
try {
    val result : PayoutAccount = apiInstance.payoutsGetAccount()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayoutsApi#payoutsGetAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayoutsApi#payoutsGetAccount")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PayoutAccount**](PayoutAccount.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="payoutsGetAccountLink"></a>
# **payoutsGetAccountLink**
> PayoutAccountLink payoutsGetAccountLink(useCase)

Create Account Link

Generate temporary links for onboarding or viewing portals.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = PayoutsApi()
val useCase : kotlin.String = useCase_example // kotlin.String | Onboarding link type context
try {
    val result : PayoutAccountLink = apiInstance.payoutsGetAccountLink(useCase)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayoutsApi#payoutsGetAccountLink")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayoutsApi#payoutsGetAccountLink")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **useCase** | **kotlin.String**| Onboarding link type context | [optional] [enum: account_onboarding, payouts_portal] |

### Return type

[**PayoutAccountLink**](PayoutAccountLink.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="payoutsGetToken"></a>
# **payoutsGetToken**
> PayoutAccessToken payoutsGetToken()

Generate Portal Access Token

Generate temporary credentials to access the embed portal.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = PayoutsApi()
try {
    val result : PayoutAccessToken = apiInstance.payoutsGetToken()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayoutsApi#payoutsGetToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayoutsApi#payoutsGetToken")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PayoutAccessToken**](PayoutAccessToken.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="payoutsGetWithdrawals"></a>
# **payoutsGetWithdrawals**
> WithdrawalList payoutsGetWithdrawals(limit, page)

Get Withdrawals List

Retrieve withdrawal records for the active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = PayoutsApi()
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Page size limit
val page : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Page number
try {
    val result : WithdrawalList = apiInstance.payoutsGetWithdrawals(limit, page)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayoutsApi#payoutsGetWithdrawals")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayoutsApi#payoutsGetWithdrawals")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **java.math.BigDecimal**| Page size limit | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **java.math.BigDecimal**| Page number | [optional] |

### Return type

[**WithdrawalList**](WithdrawalList.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="payoutsListMethods"></a>
# **payoutsListMethods**
> PayoutMethodList payoutsListMethods(limit, page)

List Payout Methods

List saved payout destinations (bank accounts, cards).

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = PayoutsApi()
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | 
val page : java.math.BigDecimal = 8.14 // java.math.BigDecimal | 
try {
    val result : PayoutMethodList = apiInstance.payoutsListMethods(limit, page)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayoutsApi#payoutsListMethods")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayoutsApi#payoutsListMethods")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **java.math.BigDecimal**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **java.math.BigDecimal**|  | [optional] |

### Return type

[**PayoutMethodList**](PayoutMethodList.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="payoutsListVerifications"></a>
# **payoutsListVerifications**
> PayoutVerificationList payoutsListVerifications(limit, page)

List Verifications

Retrieve pending or completed KYC verification checks.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = PayoutsApi()
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | 
val page : java.math.BigDecimal = 8.14 // java.math.BigDecimal | 
try {
    val result : PayoutVerificationList = apiInstance.payoutsListVerifications(limit, page)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayoutsApi#payoutsListVerifications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayoutsApi#payoutsListVerifications")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **java.math.BigDecimal**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **java.math.BigDecimal**|  | [optional] |

### Return type

[**PayoutVerificationList**](PayoutVerificationList.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="payoutsListWithdrawals"></a>
# **payoutsListWithdrawals**
> WithdrawalList payoutsListWithdrawals(limit, page)

List Withdrawals

Retrieve a list of past withdrawal history.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = PayoutsApi()
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Page size limit
val page : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Page number
try {
    val result : WithdrawalList = apiInstance.payoutsListWithdrawals(limit, page)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayoutsApi#payoutsListWithdrawals")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayoutsApi#payoutsListWithdrawals")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **java.math.BigDecimal**| Page size limit | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **java.math.BigDecimal**| Page number | [optional] |

### Return type

[**WithdrawalList**](WithdrawalList.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

