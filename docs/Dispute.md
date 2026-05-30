
# Dispute

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | The dispute ID |  |
| **whopId** | **kotlin.String** | The Whop Dispute ID |  |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The dispute amount |  |
| **currency** | **kotlin.String** | The currency code |  |
| **status** | **kotlin.String** | The status of the dispute |  |
| **editable** | **kotlin.Boolean** | Whether the evidence is still editable |  |
| **visaRdr** | **kotlin.Boolean** | Whether Visa RDR was applied |  |
| **paymentId** | **kotlin.String** | The associated payment ID |  |
| **businessId** | **kotlin.String** | The associated business ID |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the dispute was created |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the dispute was last updated |  |
| **reason** | **kotlin.String** | The reason for the dispute |  [optional] |
| **needsResponseBy** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp by when evidence must be submitted |  [optional] |
| **billingAddress** | **kotlin.String** | Customer billing address details |  [optional] |
| **customerName** | **kotlin.String** | Customer name |  [optional] |
| **customerEmail** | **kotlin.String** | Customer email address |  [optional] |
| **notes** | **kotlin.String** | Additional notes |  [optional] |
| **productDescription** | **kotlin.String** | Product or service description |  [optional] |
| **serviceDate** | **kotlin.String** | Service or purchase date |  [optional] |
| **accessActivityLog** | **kotlin.String** | Log of access activity |  [optional] |
| **evidence** | [**DisputeEvidenceDto**](DisputeEvidenceDto.md) | Evidence attachments associated with the dispute |  [optional] |



