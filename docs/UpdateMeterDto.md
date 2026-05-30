
# UpdateMeterDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Meter display name. |  [optional] |
| **description** | **kotlin.String** | Meter description. |  [optional] |
| **eventName** | **kotlin.String** | The event name tracked by this meter. |  [optional] |
| **aggregationType** | [**inline**](#AggregationType) | Aggregation strategy for usage events. |  [optional] |
| **aggregationKey** | **kotlin.String** | Metadata key used by SUM, MAX, or LAST aggregation modes. |  [optional] |
| **unit** | **kotlin.String** | Measurement unit label. |  [optional] |
| **filters** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional filter definition for advanced matching. |  [optional] |
| **enableFiltering** | **kotlin.Boolean** | Enable filtering on usage event ingestion. |  [optional] |


<a id="AggregationType"></a>
## Enum: aggregationType
| Name | Value |
| ---- | ----- |
| aggregationType | COUNT, SUM, MAX, LAST |



