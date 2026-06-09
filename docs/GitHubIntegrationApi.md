# GitHubIntegrationApi

All URIs are relative to *https://api.solifyn.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**githubGetInstallUrl**](GitHubIntegrationApi.md#githubGetInstallUrl) | **GET** /v1/github/install | Get GitHub App Installation URL |
| [**githubListRepos**](GitHubIntegrationApi.md#githubListRepos) | **GET** /v1/github/repos | List Available GitHub Repositories |


<a id="githubGetInstallUrl"></a>
# **githubGetInstallUrl**
> githubGetInstallUrl(productId)

Get GitHub App Installation URL

Generates the URL to install the system-wide GitHub App onto the merchant&#39;s GitHub account/org.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = GitHubIntegrationApi()
val productId : kotlin.String = productId_example // kotlin.String | Optional Product ID to redirect back to after installation
try {
    apiInstance.githubGetInstallUrl(productId)
} catch (e: ClientException) {
    println("4xx response calling GitHubIntegrationApi#githubGetInstallUrl")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GitHubIntegrationApi#githubGetInstallUrl")
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


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="githubListRepos"></a>
# **githubListRepos**
> kotlin.collections.List&lt;GithubReposResponseDto&gt; githubListRepos()

List Available GitHub Repositories

Retrieves all repositories accessible by the merchant&#39;s installed GitHub App.

### Example
```kotlin
// Import classes:
//import com.solifyn.infrastructure.*
//import com.solifyn.model.*

val apiInstance = GitHubIntegrationApi()
try {
    val result : kotlin.collections.List<GithubReposResponseDto> = apiInstance.githubListRepos()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GitHubIntegrationApi#githubListRepos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GitHubIntegrationApi#githubListRepos")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;GithubReposResponseDto&gt;**](GithubReposResponseDto.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

