# CollectionsApi

All URIs are relative to *http://localhost:8000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**collectionsAddProducts**](CollectionsApi.md#collectionsAddProducts) | **POST** /v1/collections/{id}/products | Add Products to Collection |
| [**collectionsArchive**](CollectionsApi.md#collectionsArchive) | **DELETE** /v1/collections/{id} | Archive Collection |
| [**collectionsCreate**](CollectionsApi.md#collectionsCreate) | **POST** /v1/collections | Create Collection |
| [**collectionsDeleteProduct**](CollectionsApi.md#collectionsDeleteProduct) | **DELETE** /v1/collections/{id}/products/{productId} | Remove Product from Collection |
| [**collectionsGet**](CollectionsApi.md#collectionsGet) | **GET** /v1/collections/{id} | Retrieve Collection |
| [**collectionsList**](CollectionsApi.md#collectionsList) | **GET** /v1/collections | List Collections |
| [**collectionsListArchived**](CollectionsApi.md#collectionsListArchived) | **GET** /v1/collections/archived | List Archived Collections |
| [**collectionsUnarchive**](CollectionsApi.md#collectionsUnarchive) | **POST** /v1/collections/{id}/unarchive | Unarchive Collection |
| [**collectionsUpdate**](CollectionsApi.md#collectionsUpdate) | **PATCH** /v1/collections/{id} | Update Collection |
| [**collectionsUpdateProduct**](CollectionsApi.md#collectionsUpdateProduct) | **PATCH** /v1/collections/{id}/products/{productId} | Update Collection Product |


<a id="collectionsAddProducts"></a>
# **collectionsAddProducts**
> CollectionResponseDto collectionsAddProducts(id, addCollectionProductsDto)

Add Products to Collection

Add one or more products to a collection. If a product already exists, its quantity is updated.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CollectionsApi()
val id : kotlin.String = col_123 // kotlin.String | Collection ID
val addCollectionProductsDto : AddCollectionProductsDto =  // AddCollectionProductsDto | 
try {
    val result : CollectionResponseDto = apiInstance.collectionsAddProducts(id, addCollectionProductsDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#collectionsAddProducts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#collectionsAddProducts")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Collection ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **addCollectionProductsDto** | [**AddCollectionProductsDto**](AddCollectionProductsDto.md)|  | |

### Return type

[**CollectionResponseDto**](CollectionResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="collectionsArchive"></a>
# **collectionsArchive**
> CollectionArchivedResponseDto collectionsArchive(id)

Archive Collection

Deactivate and move a collection to archives.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CollectionsApi()
val id : kotlin.String = col_123 // kotlin.String | Collection ID
try {
    val result : CollectionArchivedResponseDto = apiInstance.collectionsArchive(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#collectionsArchive")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#collectionsArchive")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Collection ID | |

### Return type

[**CollectionArchivedResponseDto**](CollectionArchivedResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="collectionsCreate"></a>
# **collectionsCreate**
> CollectionResponseDto collectionsCreate(createCollectionDto)

Create Collection

Generate a new product collection for checkout packaging.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CollectionsApi()
val createCollectionDto : CreateCollectionDto =  // CreateCollectionDto | 
try {
    val result : CollectionResponseDto = apiInstance.collectionsCreate(createCollectionDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#collectionsCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#collectionsCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createCollectionDto** | [**CreateCollectionDto**](CreateCollectionDto.md)|  | |

### Return type

[**CollectionResponseDto**](CollectionResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="collectionsDeleteProduct"></a>
# **collectionsDeleteProduct**
> CollectionProductDeletedResponseDto collectionsDeleteProduct(id, productId)

Remove Product from Collection

Remove a product from a collection.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CollectionsApi()
val id : kotlin.String = col_123 // kotlin.String | Collection ID
val productId : kotlin.String = prod_123 // kotlin.String | Product ID
try {
    val result : CollectionProductDeletedResponseDto = apiInstance.collectionsDeleteProduct(id, productId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#collectionsDeleteProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#collectionsDeleteProduct")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Collection ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productId** | **kotlin.String**| Product ID | |

### Return type

[**CollectionProductDeletedResponseDto**](CollectionProductDeletedResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="collectionsGet"></a>
# **collectionsGet**
> CollectionDetailResponseDto collectionsGet(id)

Retrieve Collection

Get properties of a product collection by ID.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CollectionsApi()
val id : kotlin.String = col_123 // kotlin.String | Collection ID
try {
    val result : CollectionDetailResponseDto = apiInstance.collectionsGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#collectionsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#collectionsGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Collection ID | |

### Return type

[**CollectionDetailResponseDto**](CollectionDetailResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="collectionsList"></a>
# **collectionsList**
> kotlin.collections.List&lt;CollectionResponseDto&gt; collectionsList()

List Collections

Get all active product collections linked to the current active business.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CollectionsApi()
try {
    val result : kotlin.collections.List<CollectionResponseDto> = apiInstance.collectionsList()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#collectionsList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#collectionsList")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CollectionResponseDto&gt;**](CollectionResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="collectionsListArchived"></a>
# **collectionsListArchived**
> kotlin.collections.List&lt;CollectionResponseDto&gt; collectionsListArchived()

List Archived Collections

Get all archived/deactivated product collections.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CollectionsApi()
try {
    val result : kotlin.collections.List<CollectionResponseDto> = apiInstance.collectionsListArchived()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#collectionsListArchived")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#collectionsListArchived")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CollectionResponseDto&gt;**](CollectionResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="collectionsUnarchive"></a>
# **collectionsUnarchive**
> CollectionUnarchivedResponseDto collectionsUnarchive(id)

Unarchive Collection

Restore an archived collection back to active status.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CollectionsApi()
val id : kotlin.String = col_123 // kotlin.String | Collection ID
try {
    val result : CollectionUnarchivedResponseDto = apiInstance.collectionsUnarchive(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#collectionsUnarchive")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#collectionsUnarchive")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Collection ID | |

### Return type

[**CollectionUnarchivedResponseDto**](CollectionUnarchivedResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="collectionsUpdate"></a>
# **collectionsUpdate**
> CollectionUpdatedResponseDto collectionsUpdate(id, updateCollectionDto)

Update Collection

Update products, friendly name, status, or description of a collection.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CollectionsApi()
val id : kotlin.String = col_123 // kotlin.String | Collection ID
val updateCollectionDto : UpdateCollectionDto =  // UpdateCollectionDto | 
try {
    val result : CollectionUpdatedResponseDto = apiInstance.collectionsUpdate(id, updateCollectionDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#collectionsUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#collectionsUpdate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Collection ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateCollectionDto** | [**UpdateCollectionDto**](UpdateCollectionDto.md)|  | |

### Return type

[**CollectionUpdatedResponseDto**](CollectionUpdatedResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="collectionsUpdateProduct"></a>
# **collectionsUpdateProduct**
> CollectionProductUpdatedResponseDto collectionsUpdateProduct(id, productId, updateCollectionProductDto)

Update Collection Product

Update quantity of a specific product inside a collection.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = CollectionsApi()
val id : kotlin.String = col_123 // kotlin.String | Collection ID
val productId : kotlin.String = prod_123 // kotlin.String | Product ID
val updateCollectionProductDto : UpdateCollectionProductDto =  // UpdateCollectionProductDto | 
try {
    val result : CollectionProductUpdatedResponseDto = apiInstance.collectionsUpdateProduct(id, productId, updateCollectionProductDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#collectionsUpdateProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#collectionsUpdateProduct")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Collection ID | |
| **productId** | **kotlin.String**| Product ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateCollectionProductDto** | [**UpdateCollectionProductDto**](UpdateCollectionProductDto.md)|  | |

### Return type

[**CollectionProductUpdatedResponseDto**](CollectionProductUpdatedResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

