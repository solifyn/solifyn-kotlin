
# CollectionResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) | The collection ID |  |
| **name** | **kotlin.String** | The name of the collection |  |
| **status** | [**inline**](#Status) | Status of the collection |  |
| **businessId** | **kotlin.String** | The unique identifier of the business owning this collection. |  |
| **isPermanentlyDeleted** | **kotlin.Boolean** | Indicates if the collection has been permanently deleted. |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the collection was created |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the collection was last updated |  |
| **description** | **kotlin.String** | A brief description of the collection |  [optional] |
| **imageUrl** | **kotlin.String** | URL of the collection image |  [optional] |
| **products** | [**kotlin.collections.List&lt;CollectionProductRefDto&gt;**](CollectionProductRefDto.md) | List of product references (id + quantity). Full product details are available via GET /products/:id. |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | ACTIVE, ARCHIVED |



