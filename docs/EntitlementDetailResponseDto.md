
# EntitlementDetailResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | The unique entitlement ID |  |
| **businessId** | **kotlin.String** | The owning business ID |  |
| **name** | **kotlin.String** | The name of the entitlement |  |
| **type** | **kotlin.String** | The type of access to grant |  |
| **status** | **kotlin.String** | Status of the entitlement |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the entitlement was created |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the entitlement was last updated |  |
| **grantsCount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Number of active customer grants issued from this entitlement |  |
| **products** | [**kotlin.collections.List&lt;LinkedProductDto&gt;**](LinkedProductDto.md) | Products that are currently linked to this entitlement |  |
| **githubRepo** | **kotlin.String** | The GitHub repository (e.g., owner/repo) |  [optional] |
| **githubPermission** | **kotlin.String** | The GitHub repository permission level |  [optional] |
| **discordGuildId** | **kotlin.String** | The Discord Guild/Server ID |  [optional] |
| **discordRoleId** | **kotlin.String** | The Discord Role ID to assign |  [optional] |
| **framerTemplateId** | **kotlin.String** | The associated Framer Template ID |  [optional] |
| **licenseKey** | **kotlin.String** | The static License Key (if not dynamically generated) |  [optional] |
| **activationLimit** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The maximum activation limit for licenses |  [optional] |
| **activationMessage** | **kotlin.String** | A message shown to the user upon license activation |  [optional] |
| **expiryHours** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The number of hours until the entitlement expires |  [optional] |
| **digitalLink** | **kotlin.String** | The digital download URL or redirect link |  [optional] |
| **instructions** | **kotlin.String** | Custom setup instructions for the user |  [optional] |



