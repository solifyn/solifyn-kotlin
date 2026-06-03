
# OperationalWebhookEndpointInDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **url** | **kotlin.String** | The URL to send webhook events to. |  |
| **description** | **kotlin.String** | Optional description for the endpoint. |  [optional] |
| **disabled** | **kotlin.Boolean** | Whether the endpoint is disabled. |  [optional] |
| **filterTypes** | **kotlin.collections.List&lt;kotlin.String&gt;** | The operational event types this endpoint will receive. |  [optional] |
| **metadata** | [**kotlin.Any**](.md) | Metadata key-value pairs associated with the endpoint. |  [optional] |
| **secret** | **kotlin.String** | Optional custom endpoint signing secret (base64 encoded random bytes optionally prefixed with whsec_). If not set, the server will generate one. |  [optional] |
| **throttleRate** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Maximum messages per second to send to this endpoint (outgoing messages will be throttled to this rate). |  [optional] |
| **uid** | **kotlin.String** | Optional unique user-defined identifier for the endpoint. |  [optional] |



