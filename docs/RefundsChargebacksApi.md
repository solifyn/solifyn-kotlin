# RefundsChargebacksApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**refundsCreate**](RefundsChargebacksApi.md#refundsCreate) | **POST** /v1/orders/{id}/refund | Create Refund |
| [**refundsGet**](RefundsChargebacksApi.md#refundsGet) | **GET** /v1/refunds/{id} | Retrieve Refund details |
| [**refundsList**](RefundsChargebacksApi.md#refundsList) | **GET** /v1/refunds | List Refunds |


<a id="refundsCreate"></a>
# **refundsCreate**
> refundsCreate(id, orderRefundCreate)

Create Refund

Initiate a full or partial refund for a specific payment/order.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = RefundsChargebacksApi()
val id : kotlin.String = pay_123 // kotlin.String | The unique order/payment ID.
val orderRefundCreate : OrderRefundCreate =  // OrderRefundCreate | 
try {
    apiInstance.refundsCreate(id, orderRefundCreate)
} catch (e: ClientException) {
    println("4xx response calling RefundsChargebacksApi#refundsCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RefundsChargebacksApi#refundsCreate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique order/payment ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderRefundCreate** | [**OrderRefundCreate**](OrderRefundCreate.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="refundsGet"></a>
# **refundsGet**
> Refund refundsGet(id)

Retrieve Refund details

Get parameters of a specific processed refund by database ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = RefundsChargebacksApi()
val id : kotlin.String = ref_123 // kotlin.String | Refund ID
try {
    val result : Refund = apiInstance.refundsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RefundsChargebacksApi#refundsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RefundsChargebacksApi#refundsGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Refund ID | |

### Return type

[**Refund**](Refund.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="refundsList"></a>
# **refundsList**
> kotlin.collections.List&lt;Refund&gt; refundsList()

List Refunds

Retrieve a list of processed refunds and chargeback transactions.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = RefundsChargebacksApi()
try {
    val result : kotlin.collections.List<Refund> = apiInstance.refundsList()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RefundsChargebacksApi#refundsList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RefundsChargebacksApi#refundsList")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;Refund&gt;**](Refund.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

