
# ProductCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Product display name. |  |
| **price** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Price value. |  |
| **currency** | [**inline**](#Currency) | Product pricing currency. |  |
| **taxCategory** | [**inline**](#TaxCategory) | Tax classification. |  |
| **description** | **kotlin.String** | A description of the product. |  [optional] |
| **imageUrl** | **kotlin.String** | URL of the product cover image. |  [optional] |
| **discount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Percentage or flat rate discount. |  [optional] |
| **hasLicenseKey** | **kotlin.Boolean** | Whether to automatically issue license keys upon successful orders. |  [optional] |
| **hasDigitalDelivery** | **kotlin.Boolean** | Whether the purchase includes downloadable files. |  [optional] |
| **hasGithubAccess** | **kotlin.Boolean** | Whether the purchase includes GitHub repository access. |  [optional] |
| **githubRepo** | **kotlin.String** | GitHub repository to grant access to (format: owner/repo). |  [optional] |
| **githubPermission** | [**inline**](#GithubPermission) | GitHub collaborator permission level. |  [optional] |
| **hasDiscordAccess** | **kotlin.Boolean** | Whether the purchase includes Discord server role access. |  [optional] |
| **discordGuildId** | **kotlin.String** | Discord Guild (Server) ID to grant access to. |  [optional] |
| **discordRoleId** | **kotlin.String** | Discord Role ID to assign to the user. |  [optional] |
| **isTaxInclusive** | **kotlin.Boolean** | Whether tax is included in the base price. |  [optional] |
| **activationLimit** | **kotlin.Int** | Maximum concurrent activated instances allowed per license key. |  [optional] |
| **brandId** | **kotlin.String** | Brand id for the product, if not provided will default to primary brand. |  [optional] |
| **billingPeriod** | **kotlin.Int** | Billing period in days (for Subscription products). |  [optional] |
| **trialPeriodDays** | **kotlin.Int** | Trial duration in days. |  [optional] |
| **expirationDays** | **kotlin.Int** | Subscription expiration duration in days. |  [optional] |
| **statementDescriptor** | **kotlin.String** | Custom billing descriptor. |  [optional] |
| **payWhatYouWant** | **kotlin.Boolean** | Allow pay-what-you-want pricing. |  [optional] |
| **metadata** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** | Developer key-value metadata pairs. |  [optional] |
| **customFields** | [**kotlin.collections.List&lt;ProductCreateCustomFieldsInner&gt;**](ProductCreateCustomFieldsInner.md) | Form field configurations to gather during checkout. |  [optional] |
| **stock** | **kotlin.Int** | Initial stock quantity limit. |  [optional] |
| **isListed** | **kotlin.Boolean** | Whether the product is publicly visible. |  [optional] |
| **isFree** | **kotlin.Boolean** | Whether the product is free of charge. |  [optional] |
| **addons** | [**kotlin.collections.List&lt;ProductCreateAddonsInner&gt;**](ProductCreateAddonsInner.md) | Product addons configurations. |  [optional] |
| **entitlementIds** | **kotlin.collections.List&lt;kotlin.String&gt;** | Array of independent entitlement IDs to link to this product. |  [optional] |


<a id="Currency"></a>
## Enum: currency
| Name | Value |
| ---- | ----- |
| currency | USD, SGD, INR, AUD, BRL, CAD, DKK, EUR, NOK, GBP, SEK, CHF, HKD, HUF, JPY, MXN, MYR, PLN, CZK, NZD, AED, COP, RON, THB, BGN, IDR, DOP, PHP, TRY, KRW, TWD, VND, PKR, CLP, UYU, ARS, ZAR, DZD, TND, MAD, KES, KWD, JOD, ALL, XCD, AMD, BSD, BHD, BOB, BAM, KHR, CRC, XOF, EGP, ETB, GMD, GHS, GTQ, GYD, ILS, JMD, MOP, MGA, MUR, MDL, MNT, NAD, NGN, MKD, OMR, PYG, PEN, QAR, RWF, SAR, RSD, LKR, TZS, TTD, UZS, RUB, CNY |


<a id="TaxCategory"></a>
## Enum: taxCategory
| Name | Value |
| ---- | ----- |
| taxCategory | digital_products, saas, physical_products, service |


<a id="GithubPermission"></a>
## Enum: githubPermission
| Name | Value |
| ---- | ----- |
| githubPermission | pull, triage, push, maintain, admin |



