# DiscordIntegrationApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**discordGetInstallUrl**](DiscordIntegrationApi.md#discordGetInstallUrl) | **GET** /v1/discord/install | Get Discord Bot Installation URL |
| [**discordListRoles**](DiscordIntegrationApi.md#discordListRoles) | **GET** /v1/discord/roles | List Guild Discord Roles |


<a id="discordGetInstallUrl"></a>
# **discordGetInstallUrl**
> discordGetInstallUrl(productId)

Get Discord Bot Installation URL

Generates the URL to invite the system-wide Discord Bot onto the merchant&#39;s Discord server.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DiscordIntegrationApi()
val productId : kotlin.String = productId_example // kotlin.String | Optional Product ID to redirect back to after installation
try {
    apiInstance.discordGetInstallUrl(productId)
} catch (e: ClientException) {
    println("4xx response calling DiscordIntegrationApi#discordGetInstallUrl")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DiscordIntegrationApi#discordGetInstallUrl")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productId** | **kotlin.String**| Optional Product ID to redirect back to after installation | [optional] |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="discordListRoles"></a>
# **discordListRoles**
> kotlin.collections.List&lt;DiscordRolesResponseDto&gt; discordListRoles()

List Guild Discord Roles

Retrieves all roles available in the connected merchant&#39;s Discord server/guild.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = DiscordIntegrationApi()
try {
    val result : kotlin.collections.List<DiscordRolesResponseDto> = apiInstance.discordListRoles()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DiscordIntegrationApi#discordListRoles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DiscordIntegrationApi#discordListRoles")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;DiscordRolesResponseDto&gt;**](DiscordRolesResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

