
# MeterUsageEventDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | The unique usage event ID. |  |
| **meterId** | **kotlin.String** | The meter ID this event belongs to. |  |
| **customerId** | **kotlin.String** | The customer ID associated with the usage event. |  |
| **&#x60;value&#x60;** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Numeric usage value recorded for the event. |  |
| **timestamp** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the usage event occurred. |  |
| **processedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the usage event was processed. |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional event metadata. |  [optional] |



