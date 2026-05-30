
# MeterIngestEventDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **eventId** | **kotlin.String** | Unique usage event ID for idempotency. |  |
| **customerId** | **kotlin.String** | Unique customer ID associated with the event. |  |
| **eventName** | **kotlin.String** | Event name that should match a meter eventName. |  |
| **&#x60;value&#x60;** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Event quantity value. |  [optional] |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Metadata attached to the usage event. |  [optional] |
| **timestamp** | **kotlin.String** | Timestamp of the event in ISO 8601 format. |  [optional] |



