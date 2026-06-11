
# CreateEntitlementDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | The user-friendly name of the entitlement |  |
| **type** | [**inline**](#Type) | The type of access to grant |  |
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


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | GITHUB, DISCORD, FRAMER, LICENSE, DIGITAL |



