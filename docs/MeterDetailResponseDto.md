
# MeterDetailResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | The unique meter ID. |  |
| **businessId** | **kotlin.String** | The business ID that owns this meter. |  |
| **name** | **kotlin.String** | Meter display name. |  |
| **eventName** | **kotlin.String** | The event name tracked by this meter. |  |
| **aggregationType** | [**inline**](#AggregationType) | Aggregation strategy for usage events. |  |
| **archived** | **kotlin.Boolean** | Whether the meter is archived. |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Creation timestamp. |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Last update timestamp. |  |
| **usageEvents** | [**kotlin.collections.List&lt;MeterUsageEventDto&gt;**](MeterUsageEventDto.md) | Most recent usage events recorded for the meter. |  |
| **totalUsageEvents** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Total usage event count for the meter. |  |
| **description** | [**kotlin.Any**](.md) | Meter description. |  [optional] |
| **aggregationKey** | [**kotlin.Any**](.md) | Metadata key used for aggregation. |  [optional] |
| **unit** | [**kotlin.Any**](.md) | Measurement unit label. |  [optional] |
| **filters** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional filter definition for advanced matching. |  [optional] |


<a id="AggregationType"></a>
## Enum: aggregationType
| Name | Value |
| ---- | ----- |
| aggregationType | COUNT, SUM, MAX, LAST |



