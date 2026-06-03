# DefaultApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**disputeCreatedPost**](DefaultApi.md#disputeCreatedPost) | **POST** /dispute.created | Dispute Created |
| [**disputeLostPost**](DefaultApi.md#disputeLostPost) | **POST** /dispute.lost | Dispute Lost |
| [**disputeWonPost**](DefaultApi.md#disputeWonPost) | **POST** /dispute.won | Dispute Won |
| [**licenseCreatedPost**](DefaultApi.md#licenseCreatedPost) | **POST** /license.created | License Created |
| [**licenseRevokedPost**](DefaultApi.md#licenseRevokedPost) | **POST** /license.revoked | License Revoked |
| [**paymentCreatedPost**](DefaultApi.md#paymentCreatedPost) | **POST** /payment.created | Payment Created |
| [**paymentFailedPost**](DefaultApi.md#paymentFailedPost) | **POST** /payment.failed | Payment Failed |
| [**paymentSucceededPost**](DefaultApi.md#paymentSucceededPost) | **POST** /payment.succeeded | Payment Succeeded |
| [**refundFailedPost**](DefaultApi.md#refundFailedPost) | **POST** /refund.failed | Refund Failed |
| [**refundSucceededPost**](DefaultApi.md#refundSucceededPost) | **POST** /refund.succeeded | Refund Succeeded |
| [**subscriptionCreatedPost**](DefaultApi.md#subscriptionCreatedPost) | **POST** /subscription.created | Subscription Created |
| [**subscriptionDeactivatedPost**](DefaultApi.md#subscriptionDeactivatedPost) | **POST** /subscription.deactivated | Subscription Deactivated |
| [**subscriptionUpdatedPost**](DefaultApi.md#subscriptionUpdatedPost) | **POST** /subscription.updated | Subscription Updated |


<a id="disputeCreatedPost"></a>
# **disputeCreatedPost**
> disputeCreatedPost(webhookDisputePayload)

Dispute Created

Occurs when a payment charge is disputed by the customer (chargeback initiated).

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookDisputePayload : WebhookDisputePayload =  // WebhookDisputePayload | 
try {
    apiInstance.disputeCreatedPost(webhookDisputePayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#disputeCreatedPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#disputeCreatedPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookDisputePayload** | [**WebhookDisputePayload**](WebhookDisputePayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="disputeLostPost"></a>
# **disputeLostPost**
> disputeLostPost(webhookDisputePayload)

Dispute Lost

Occurs when a dispute challenge is lost and the funds are returned to the cardholder.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookDisputePayload : WebhookDisputePayload =  // WebhookDisputePayload | 
try {
    apiInstance.disputeLostPost(webhookDisputePayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#disputeLostPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#disputeLostPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookDisputePayload** | [**WebhookDisputePayload**](WebhookDisputePayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="disputeWonPost"></a>
# **disputeWonPost**
> disputeWonPost(webhookDisputePayload)

Dispute Won

Occurs when a dispute challenge is won by the merchant.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookDisputePayload : WebhookDisputePayload =  // WebhookDisputePayload | 
try {
    apiInstance.disputeWonPost(webhookDisputePayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#disputeWonPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#disputeWonPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookDisputePayload** | [**WebhookDisputePayload**](WebhookDisputePayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="licenseCreatedPost"></a>
# **licenseCreatedPost**
> licenseCreatedPost(webhookLicensePayload)

License Created

Occurs when a new software license key is created or assigned to a customer purchase.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookLicensePayload : WebhookLicensePayload =  // WebhookLicensePayload | 
try {
    apiInstance.licenseCreatedPost(webhookLicensePayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#licenseCreatedPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#licenseCreatedPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookLicensePayload** | [**WebhookLicensePayload**](WebhookLicensePayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="licenseRevokedPost"></a>
# **licenseRevokedPost**
> licenseRevokedPost(webhookLicensePayload)

License Revoked

Occurs when a software license key is revoked (e.g., due to subscription cancellation, refund, or dispute).

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookLicensePayload : WebhookLicensePayload =  // WebhookLicensePayload | 
try {
    apiInstance.licenseRevokedPost(webhookLicensePayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#licenseRevokedPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#licenseRevokedPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookLicensePayload** | [**WebhookLicensePayload**](WebhookLicensePayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="paymentCreatedPost"></a>
# **paymentCreatedPost**
> paymentCreatedPost(webhookPaymentPayload)

Payment Created

Occurs when a new payment is initiated (e.g., at checkout start or subscription creation). The payment may still be in an incomplete or pending state.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookPaymentPayload : WebhookPaymentPayload = {"id":"pay_123","status":"created","substatus":"incomplete","customerId":"usr_123","customerEmail":"customer@example.com","customerName":"John Doe","customerUsername":"johndoe","productTitle":"SaaS Pro Access","productRoute":"saas-pro-access","planId":"plan_123","membershipId":"mem_123","membershipStatus":"drafted","billingReason":"subscription_create","amount":"29.00","subtotal":"29.00","usdTotal":"29.00","feeAmount":"1.50","amountAfterFees":"27.50","taxAmount":null,"taxBehavior":null,"taxRefundedAmount":null,"refundedAmount":"0","settlementAmount":"29.00","settlementCurrency":"usd","settlementExchangeRate":null,"currency":"USD","refundable":false,"retryable":false,"autoRefunded":false,"paymentMethod":null,"cardBrand":null,"cardLast4":null,"cardExpMonth":null,"cardExpYear":null,"billingAddress":{"name":"John Doe","line1":"123 Main St","line2":"","city":"San Francisco","state":"CA","country":"US","postal_code":"94105"},"licenseKey":null,"filesSnapshot":null,"checkoutId":null,"discountCode":null,"failureMessage":null,"paidAt":"2026-05-25T20:20:05.000Z","refundedAt":null,"disputeAlertedAt":null,"lastPaymentAttempt":null,"nextPaymentAttempt":"2026-05-25T20:20:05.000Z","createdAt":"2026-05-25T20:20:06.000Z","updatedAt":"2026-05-25T20:20:06.000Z","paymentEventType":"payment.created","lastEventType":"payment.created","businessId":"biz_123"} // WebhookPaymentPayload | 
try {
    apiInstance.paymentCreatedPost(webhookPaymentPayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#paymentCreatedPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#paymentCreatedPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookPaymentPayload** | [**WebhookPaymentPayload**](WebhookPaymentPayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="paymentFailedPost"></a>
# **paymentFailedPost**
> paymentFailedPost(order)

Payment Failed

Occurs when a customer payment attempt fails.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val order : Order =  // Order | 
try {
    apiInstance.paymentFailedPost(order)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#paymentFailedPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#paymentFailedPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order** | [**Order**](Order.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="paymentSucceededPost"></a>
# **paymentSucceededPost**
> paymentSucceededPost(order)

Payment Succeeded

Occurs when a customer payment is confirmed as succeeded.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val order : Order =  // Order | 
try {
    apiInstance.paymentSucceededPost(order)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#paymentSucceededPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#paymentSucceededPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order** | [**Order**](Order.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="refundFailedPost"></a>
# **refundFailedPost**
> refundFailedPost(webhookRefundPayload)

Refund Failed

Occurs when a payment refund fails.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookRefundPayload : WebhookRefundPayload =  // WebhookRefundPayload | 
try {
    apiInstance.refundFailedPost(webhookRefundPayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#refundFailedPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#refundFailedPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookRefundPayload** | [**WebhookRefundPayload**](WebhookRefundPayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="refundSucceededPost"></a>
# **refundSucceededPost**
> refundSucceededPost(webhookRefundPayload)

Refund Succeeded

Occurs when a payment refund is confirmed as succeeded.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookRefundPayload : WebhookRefundPayload =  // WebhookRefundPayload | 
try {
    apiInstance.refundSucceededPost(webhookRefundPayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#refundSucceededPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#refundSucceededPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookRefundPayload** | [**WebhookRefundPayload**](WebhookRefundPayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="subscriptionCreatedPost"></a>
# **subscriptionCreatedPost**
> subscriptionCreatedPost(webhookSubscriptionPayload)

Subscription Created

Occurs when a customer subscription is successfully started.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookSubscriptionPayload : WebhookSubscriptionPayload =  // WebhookSubscriptionPayload | 
try {
    apiInstance.subscriptionCreatedPost(webhookSubscriptionPayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#subscriptionCreatedPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#subscriptionCreatedPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookSubscriptionPayload** | [**WebhookSubscriptionPayload**](WebhookSubscriptionPayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="subscriptionDeactivatedPost"></a>
# **subscriptionDeactivatedPost**
> subscriptionDeactivatedPost(webhookSubscriptionPayload)

Subscription Deactivated

Occurs when a customer subscription is deactivated or expired.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookSubscriptionPayload : WebhookSubscriptionPayload =  // WebhookSubscriptionPayload | 
try {
    apiInstance.subscriptionDeactivatedPost(webhookSubscriptionPayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#subscriptionDeactivatedPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#subscriptionDeactivatedPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookSubscriptionPayload** | [**WebhookSubscriptionPayload**](WebhookSubscriptionPayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="subscriptionUpdatedPost"></a>
# **subscriptionUpdatedPost**
> subscriptionUpdatedPost(webhookSubscriptionPayload)

Subscription Updated

Occurs when a customer subscription is updated (e.g., cancel at period end changes).

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DefaultApi()
val webhookSubscriptionPayload : WebhookSubscriptionPayload =  // WebhookSubscriptionPayload | 
try {
    apiInstance.subscriptionUpdatedPost(webhookSubscriptionPayload)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#subscriptionUpdatedPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#subscriptionUpdatedPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookSubscriptionPayload** | [**WebhookSubscriptionPayload**](WebhookSubscriptionPayload.md)|  | [optional] |

### Return type

null (empty response body)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

