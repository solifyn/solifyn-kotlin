
# UpdateWebhookEndpointDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **url** | **kotlin.String** | The URL to send webhook events to. |  [optional] |
| **description** | **kotlin.String** | Optional description for the webhook endpoint. |  [optional] |
| **events** | **kotlin.collections.List&lt;kotlin.String&gt;** | The list of subscribed event types. |  [optional] |
| **status** | [**inline**](#Status) | The status of the webhook endpoint. |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | ACTIVE, INACTIVE |



