
# Subscription

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | The unique ID of the subscription |  |
| **status** | **kotlin.String** | The status of the subscription (e.g. completed, active, trialing, past_due, canceled) |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the subscription was created |  |
| **joinedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the member joined |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the subscription was last updated |  |
| **manageUrl** | **kotlin.String** | The management URL for the billing/subscription |  |
| **member** | [**SubscriptionMemberDto**](SubscriptionMemberDto.md) | The member details |  |
| **user** | [**SubscriptionUserDto**](SubscriptionUserDto.md) | The user details |  |
| **renewalPeriodStart** | [**kotlin.Any**](.md) | Start timestamp of the current renewal period |  |
| **renewalPeriodEnd** | [**kotlin.Any**](.md) | End timestamp of the current renewal period |  |
| **cancelAtPeriodEnd** | **kotlin.Boolean** | Whether the subscription is set to cancel at the end of the billing period |  |
| **cancelOption** | [**kotlin.Any**](.md) | The cancel option details |  |
| **cancellationReason** | [**kotlin.Any**](.md) | The reason for cancellation |  |
| **canceledAt** | [**kotlin.Any**](.md) | Timestamp when the subscription was canceled |  |
| **currency** | **kotlin.String** | The currency used for payments |  |
| **company** | [**SubscriptionCompanyDto**](SubscriptionCompanyDto.md) | The company context details |  |
| **plan** | [**SubscriptionPlanDto**](SubscriptionPlanDto.md) | The plan associated with this subscription |  |
| **promoCode** | [**kotlin.Any**](.md) | The promo code applied to the subscription |  |
| **product** | [**SubscriptionProductDto**](SubscriptionProductDto.md) | The product associated with the subscription |  |
| **licenseKey** | [**kotlin.Any**](.md) | The license key associated with this subscription |  |
| **metadata** | [**kotlin.Any**](.md) | Additional metadata for the subscription |  |
| **paymentCollectionPaused** | **kotlin.Boolean** | Whether the payment collection is currently paused |  |
| **checkoutConfigurationId** | **kotlin.String** | The checkout configuration ID used |  |
| **price** | [**kotlin.Any**](.md) | The price/amount of the membership |  [optional] |
| **type** | [**kotlin.Any**](.md) | The type of the membership plan |  [optional] |
| **customerId** | [**kotlin.Any**](.md) | The business customer ID |  [optional] |



