
# Product

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) | The unique identifier (ID) of the product. |  |
| **name** | **kotlin.String** | The display name of the product. |  |
| **price** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The price amount of the product (e.g. 29.00). |  |
| **currency** | **kotlin.String** | The three-letter ISO currency code (e.g. USD, VND, EUR). |  |
| **status** | **kotlin.String** | The lifecycle status of the product (e.g. ACTIVE, ARCHIVED). |  |
| **imageUrl** | **kotlin.String** | URL of the product cover image. |  |
| **taxCategory** | [**inline**](#TaxCategory) | The tax classification for the product. |  |
| **pricingType** | [**inline**](#PricingType) | Pricing model of the product. |  |
| **discount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Discount value as a percentage or fixed amount. |  |
| **hasLicenseKey** | **kotlin.Boolean** | Indicates if the product issues a cryptographically secure software license key upon checkout completion. |  |
| **hasDigitalDelivery** | **kotlin.Boolean** | Whether the product includes digital file downloads upon purchase. |  |
| **hasGithubAccess** | **kotlin.Boolean** | Whether the product includes GitHub repository access. |  |
| **githubRepo** | **kotlin.String** | GitHub repository to grant access to (format: owner/repo). |  |
| **githubPermission** | [**inline**](#GithubPermission) | GitHub collaborator permission level. |  |
| **hasDiscordAccess** | **kotlin.Boolean** | Whether the product includes Discord role access. |  |
| **discordGuildId** | **kotlin.String** | Discord Guild (Server) ID to grant access to. |  |
| **discordRoleId** | **kotlin.String** | Discord Role ID to assign to the user. |  |
| **isTaxInclusive** | **kotlin.Boolean** | Whether the product price already includes applicable sales taxes. |  |
| **billingPeriod** | **kotlin.Int** | The subscription billing cycle interval in days (for subscription products). |  |
| **trialPeriodDays** | **kotlin.Int** | Trial duration in days for subscription products. |  |
| **expirationDays** | **kotlin.Int** | Automatic expiration period in days for the subscription entitlement. |  |
| **statementDescriptor** | **kotlin.String** | Custom text displayed on customer credit card statements for purchases of this product. |  |
| **payWhatYouWant** | **kotlin.Boolean** | Indicates if customers are allowed to enter a custom pricing amount at checkout. |  |
| **metadata** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** | Custom developer metadata key-value pairs associated with the product. |  |
| **customFields** | [**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md) | Custom form field questions to ask the customer during checkout. |  |
| **stock** | **kotlin.Int** | Available stock quantity, or null for unlimited inventory. |  |
| **activationLimit** | **kotlin.Int** | Maximum number of simultaneous active instances/devices allowed per issued license key (applicable if hasLicenseKey is true). |  |
| **isListed** | **kotlin.Boolean** | Defines if the product is listed publicly on the merchant&#39;s storefront template. |  |
| **isFree** | **kotlin.Boolean** | Whether the product is free. |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp indicating exactly when the product was created. |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp indicating when the product was last modified. |  |
| **isPermanentlyDeleted** | **kotlin.Boolean** | Indicates if the product has been permanently deleted. |  |
| **brandId** | **kotlin.String** | Optional brand identifier. |  |
| **digitalLink** | **kotlin.String** | Secure link for digital delivery. |  |
| **instructions** | **kotlin.String** | Special instructions provided upon purchase. |  |
| **activationMessage** | **kotlin.String** | Custom message displayed when a license key is activated. |  |
| **expiryHours** | **kotlin.Int** | Number of hours until the license key expires. |  |
| **businessId** | **kotlin.String** | The unique identifier of the business owning this product. |  |
| **description** | **kotlin.String** | A comprehensive rich text description of the product. |  [optional] |


<a id="TaxCategory"></a>
## Enum: taxCategory
| Name | Value |
| ---- | ----- |
| taxCategory | digital_products, saas, physical_products, service |


<a id="PricingType"></a>
## Enum: pricingType
| Name | Value |
| ---- | ----- |
| pricingType | usage_based, one_time, renewal |


<a id="GithubPermission"></a>
## Enum: githubPermission
| Name | Value |
| ---- | ----- |
| githubPermission | pull, triage, push, maintain, admin |



