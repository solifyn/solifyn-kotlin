
# WebhookEndpointResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  |
| **url** | **kotlin.String** |  |  |
| **description** | **kotlin.String** |  |  |
| **events** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  |
| **status** | **kotlin.String** |  |  |
| **maskedSecret** | **kotlin.String** | Masked signing secret for verification. |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **secret** | **kotlin.String** | Raw signing secret (only returned once during creation). |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |



