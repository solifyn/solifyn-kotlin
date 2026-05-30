
# OrderRefundCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **amount** | **kotlin.Int** | The refund amount in cents. If full refund is true, this can represent the total amount. |  |
| **isFullRefund** | **kotlin.Boolean** | Whether this is a full refund or a partial refund. |  |
| **idempotencyKey** | **kotlin.String** | A unique idempotency key to prevent double refunds for transient network retries. |  |
| **autoRevokeSeats** | **kotlin.Boolean** | Whether to automatically revoke seat add-ons matching the refund amount. |  [optional] |
| **revokeSeats** | [**kotlin.collections.List&lt;RevokeSeatDto&gt;**](RevokeSeatDto.md) | List of specific addons and the quantities of seats to revoke. |  [optional] |



