# SubscriptionsApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**subscriptionsAction**](SubscriptionsApi.md#subscriptionsAction) | **POST** /v1/subscriptions/{subscriptionId}/{action} | Subscription Action |
| [**subscriptionsGet**](SubscriptionsApi.md#subscriptionsGet) | **GET** /v1/subscriptions/{id} | Retrieve Subscription Details |
| [**subscriptionsList**](SubscriptionsApi.md#subscriptionsList) | **GET** /v1/subscriptions | List Subscriptions |


<a id="subscriptionsAction"></a>
# **subscriptionsAction**
> SubscriptionsAction201Response subscriptionsAction(subscriptionId, action, subscriptionAction)

Subscription Action

Cancel, pause, resume, or add free days to a customer subscription.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = SubscriptionsApi()
val subscriptionId : kotlin.String = mem_123 // kotlin.String | The customer subscription ID
val action : kotlin.String = action_example // kotlin.String | The subscription task to execute
val subscriptionAction : SubscriptionAction =  // SubscriptionAction | 
try {
    val result : SubscriptionsAction201Response = apiInstance.subscriptionsAction(subscriptionId, action, subscriptionAction)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscriptionsApi#subscriptionsAction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscriptionsApi#subscriptionsAction")
    e.printStackTrace()
}
```

### Parameters
| **subscriptionId** | **kotlin.String**| The customer subscription ID | |
| **action** | **kotlin.String**| The subscription task to execute | [enum: add_free_days, cancel, pause, resume, uncancel, adjust_seats] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subscriptionAction** | [**SubscriptionAction**](SubscriptionAction.md)|  | |

### Return type

[**SubscriptionsAction201Response**](SubscriptionsAction201Response.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="subscriptionsGet"></a>
# **subscriptionsGet**
> SubscriptionDetail subscriptionsGet(id)

Retrieve Subscription Details

Retrieve detailed information about a subscription and its billing history.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = SubscriptionsApi()
val id : kotlin.String = mem_123 // kotlin.String | The customer subscription ID
try {
    val result : SubscriptionDetail = apiInstance.subscriptionsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscriptionsApi#subscriptionsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscriptionsApi#subscriptionsGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The customer subscription ID | |

### Return type

[**SubscriptionDetail**](SubscriptionDetail.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="subscriptionsList"></a>
# **subscriptionsList**
> SubscriptionList subscriptionsList(customerId)

List Subscriptions

Retrieve a list of customer subscriptions, optionally filtered by customer ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = SubscriptionsApi()
val customerId : kotlin.String = customerId_example // kotlin.String | Filter subscriptions by customer ID.
try {
    val result : SubscriptionList = apiInstance.subscriptionsList(customerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscriptionsApi#subscriptionsList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscriptionsApi#subscriptionsList")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerId** | **kotlin.String**| Filter subscriptions by customer ID. | [optional] |

### Return type

[**SubscriptionList**](SubscriptionList.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

