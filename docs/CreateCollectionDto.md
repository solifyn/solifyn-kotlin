
# CreateCollectionDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | The friendly name of the collection |  |
| **products** | [**kotlin.collections.List&lt;CollectionProductEntry&gt;**](CollectionProductEntry.md) | List of products to include in this collection. At least one product is required. |  |
| **description** | **kotlin.String** | A detailed description of this collection |  [optional] |
| **imageUrl** | **kotlin.String** | The display cover image URL for this collection |  [optional] |
| **status** | [**inline**](#Status) | The collection status |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | ACTIVE, ARCHIVED |



