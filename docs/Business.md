
# Business

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | The unique business ID |  |
| **title** | **kotlin.String** | Title or name of the business |  |
| **whopId** | **kotlin.String** | The Whop Company ID |  |
| **merchantId** | **kotlin.String** | The merchant owner ID |  |
| **verified** | **kotlin.Boolean** | Whether the business has been KYC-verified on Whop |  |
| **sendCustomerEmails** | **kotlin.Boolean** | Whether auto-emails are enabled for customers |  |
| **memberCount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Total members/customers under this business |  |
| **defaultCurrency** | **kotlin.String** | The default currency of the business |  |
| **publishedReviewsCount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Number of published user reviews on Whop |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the business record was created |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the business record was last updated |  |
| **description** | **kotlin.String** | A description explaining what the business does |  [optional] |
| **route** | **kotlin.String** | Whop friendly URL path route |  [optional] |
| **metadata** | [**kotlin.Any**](.md) | Custom key-value metadata |  [optional] |
| **targetAudience** | **kotlin.String** | The target audience description |  [optional] |
| **socialLinks** | [**kotlin.Any**](.md) | Social links setup |  [optional] |
| **affiliateInstructions** | **kotlin.String** | Markdown instructions for affiliates |  [optional] |
| **whopCreatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Whop account creation timestamp |  [optional] |
| **whopUpdatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Whop account last updated timestamp |  [optional] |
| **logoUrl** | **kotlin.String** | Brand logo image URL resolved from primary brand |  [optional] |



