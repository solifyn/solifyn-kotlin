# OrdersApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**ordersGet**](OrdersApi.md#ordersGet) | **GET** /v1/orders/{id} | Retrieve Order |
| [**ordersGetInvoice**](OrdersApi.md#ordersGetInvoice) | **GET** /v1/orders/{id}/invoice | Get Order Invoice |
| [**ordersList**](OrdersApi.md#ordersList) | **GET** /v1/orders | List Orders |
| [**ordersUpdate**](OrdersApi.md#ordersUpdate) | **PATCH** /v1/orders/{id} | Update Order Billing Address |
| [**refundsCreate**](OrdersApi.md#refundsCreate) | **POST** /v1/orders/{id}/refund | Create Refund |


<a id="ordersGet"></a>
# **ordersGet**
> Order ordersGet(id)

Retrieve Order

Retrieve details of a specific order/payment by ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = OrdersApi()
val id : kotlin.String = pay_123 // kotlin.String | The unique order/payment ID.
try {
    val result : Order = apiInstance.ordersGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#ordersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#ordersGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique order/payment ID. | |

### Return type

[**Order**](Order.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="ordersGetInvoice"></a>
# **ordersGetInvoice**
> Invoice ordersGetInvoice(id)

Get Order Invoice

Retrieve the generated invoice details for the specified order.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = OrdersApi()
val id : kotlin.String = pay_123 // kotlin.String | The unique order/payment ID.
try {
    val result : Invoice = apiInstance.ordersGetInvoice(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#ordersGetInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#ordersGetInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique order/payment ID. | |

### Return type

[**Invoice**](Invoice.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="ordersList"></a>
# **ordersList**
> OrderList ordersList(createdAtLte, createdAtGte, productId, customerId, status, pageSize, pageNumber)

List Orders

List and query orders/payments belonging to your active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = OrdersApi()
val createdAtLte : kotlin.String = createdAtLte_example // kotlin.String | Filter by creation date less than or equal to.
val createdAtGte : kotlin.String = createdAtGte_example // kotlin.String | Filter by creation date greater than or equal to.
val productId : kotlin.String = productId_example // kotlin.String | Filter by product identifier.
val customerId : kotlin.String = customerId_example // kotlin.String | Filter by customer identifier.
val status : kotlin.String = status_example // kotlin.String | Filter by order/payment status.
val pageSize : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Size of a page, defaults to 10. Maximum is 100.
val pageNumber : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Page number, defaults to 1.
try {
    val result : OrderList = apiInstance.ordersList(createdAtLte, createdAtGte, productId, customerId, status, pageSize, pageNumber)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#ordersList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#ordersList")
    e.printStackTrace()
}
```

### Parameters
| **createdAtLte** | **kotlin.String**| Filter by creation date less than or equal to. | [optional] |
| **createdAtGte** | **kotlin.String**| Filter by creation date greater than or equal to. | [optional] |
| **productId** | **kotlin.String**| Filter by product identifier. | [optional] |
| **customerId** | **kotlin.String**| Filter by customer identifier. | [optional] |
| **status** | **kotlin.String**| Filter by order/payment status. | [optional] |
| **pageSize** | **java.math.BigDecimal**| Size of a page, defaults to 10. Maximum is 100. | [optional] [default to 10] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageNumber** | **java.math.BigDecimal**| Page number, defaults to 1. | [optional] [default to 1] |

### Return type

[**OrderList**](OrderList.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="ordersUpdate"></a>
# **ordersUpdate**
> Order ordersUpdate(id, orderUpdate)

Update Order Billing Address

Update the billing details of an existing order.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = OrdersApi()
val id : kotlin.String = pay_123 // kotlin.String | The unique order/payment ID.
val orderUpdate : OrderUpdate =  // OrderUpdate | 
try {
    val result : Order = apiInstance.ordersUpdate(id, orderUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#ordersUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#ordersUpdate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique order/payment ID. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderUpdate** | [**OrderUpdate**](OrderUpdate.md)|  | |

### Return type

[**Order**](Order.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

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

val apiInstance = OrdersApi()
val id : kotlin.String = pay_123 // kotlin.String | The unique order/payment ID.
val orderRefundCreate : OrderRefundCreate =  // OrderRefundCreate | 
try {
    apiInstance.refundsCreate(id, orderRefundCreate)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#refundsCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#refundsCreate")
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

