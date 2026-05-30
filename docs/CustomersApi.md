# CustomersApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**customersCreate**](CustomersApi.md#customersCreate) | **POST** /v1/customers | Create Customer |
| [**customersGenerateInvite**](CustomersApi.md#customersGenerateInvite) | **POST** /v1/customers/{id}/share | Generate Shared Invite |
| [**customersGet**](CustomersApi.md#customersGet) | **GET** /v1/customers/{id} | Retrieve Customer |
| [**customersList**](CustomersApi.md#customersList) | **GET** /v1/customers | List Customers |
| [**customersUpdate**](CustomersApi.md#customersUpdate) | **PATCH** /v1/customers/{id} | Update Customer |


<a id="customersCreate"></a>
# **customersCreate**
> CustomerResponseDto customersCreate(createCustomerDto)

Create Customer

Add/upsert a new customer profile under the current business context.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CustomersApi()
val createCustomerDto : CreateCustomerDto =  // CreateCustomerDto | 
try {
    val result : CustomerResponseDto = apiInstance.customersCreate(createCustomerDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#customersCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#customersCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createCustomerDto** | [**CreateCustomerDto**](CreateCustomerDto.md)|  | |

### Return type

[**CustomerResponseDto**](CustomerResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="customersGenerateInvite"></a>
# **customersGenerateInvite**
> CustomerSharedInviteResponseDto customersGenerateInvite(id)

Generate Shared Invite

Generate a short-lived token granting temporary customer self-service billing page access.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CustomersApi()
val id : kotlin.String = user_123 // kotlin.String | Customer ID
try {
    val result : CustomerSharedInviteResponseDto = apiInstance.customersGenerateInvite(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#customersGenerateInvite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#customersGenerateInvite")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Customer ID | |

### Return type

[**CustomerSharedInviteResponseDto**](CustomerSharedInviteResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="customersGet"></a>
# **customersGet**
> CustomerResponseDto customersGet(id)

Retrieve Customer

Retrieve details of a customer profile by ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CustomersApi()
val id : kotlin.String = user_123 // kotlin.String | Customer ID
try {
    val result : CustomerResponseDto = apiInstance.customersGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#customersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#customersGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Customer ID | |

### Return type

[**CustomerResponseDto**](CustomerResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="customersList"></a>
# **customersList**
> CustomerListResponseDto customersList()

List Customers

Retrieve all customers associated with the current active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CustomersApi()
try {
    val result : CustomerListResponseDto = apiInstance.customersList()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#customersList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#customersList")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CustomerListResponseDto**](CustomerListResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="customersUpdate"></a>
# **customersUpdate**
> CustomerMessageResponseDto customersUpdate(id, updateCustomerDto)

Update Customer

Update name, phone, or metadata of an existing customer profile.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CustomersApi()
val id : kotlin.String = user_123 // kotlin.String | Customer ID
val updateCustomerDto : UpdateCustomerDto =  // UpdateCustomerDto | 
try {
    val result : CustomerMessageResponseDto = apiInstance.customersUpdate(id, updateCustomerDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#customersUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#customersUpdate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Customer ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateCustomerDto** | [**UpdateCustomerDto**](UpdateCustomerDto.md)|  | |

### Return type

[**CustomerMessageResponseDto**](CustomerMessageResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

