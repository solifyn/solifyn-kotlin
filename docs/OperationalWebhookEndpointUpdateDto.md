
# OperationalWebhookEndpointUpdateDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **url** | **kotlin.String** | The URL to send webhook events to. |  |
| **description** | **kotlin.String** | Optional description for the endpoint. |  [optional] |
| **disabled** | **kotlin.Boolean** | Whether the endpoint is disabled. |  [optional] |
| **filterTypes** | **kotlin.collections.List&lt;kotlin.String&gt;** | The operational event types this endpoint will receive. |  [optional] |
| **metadata** | [**kotlin.Any**](.md) | Metadata key-value pairs associated with the endpoint. |  [optional] |
| **throttleRate** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Maximum messages per second to send to this endpoint. |  [optional] |
| **uid** | **kotlin.String** | Optional unique user-defined identifier for the endpoint. |  [optional] |



