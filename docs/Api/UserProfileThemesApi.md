# Solifyn\UserProfileThemesApi

All URIs are relative to http://localhost:8000, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**usersGetMyPage()**](UserProfileThemesApi.md#usersGetMyPage) | **GET** /v1/user/my-page | Get My Page details |
| [**usersGetMyTheme()**](UserProfileThemesApi.md#usersGetMyTheme) | **GET** /v1/user/my-theme | Get My Theme |
| [**usersGetSettings()**](UserProfileThemesApi.md#usersGetSettings) | **GET** /v1/user/settings | Retrieve User Settings |
| [**usersGetStats()**](UserProfileThemesApi.md#usersGetStats) | **GET** /v1/user/dashboard-stats | Get Dashboard Statistics |
| [**usersGetThemeBySubdomain()**](UserProfileThemesApi.md#usersGetThemeBySubdomain) | **GET** /v1/user/theme/{subdomain} | Get Theme by Subdomain |


## `usersGetMyPage()`

```php
usersGetMyPage(): \Solifyn\Model\UserPage
```

Get My Page details

Retrieve page settings and custom content configured for the store.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\UserProfileThemesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->usersGetMyPage();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserProfileThemesApi->usersGetMyPage: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\Solifyn\Model\UserPage**](../Model/UserPage.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `usersGetMyTheme()`

```php
usersGetMyTheme(): \Solifyn\Model\UserTheme
```

Get My Theme

Retrieve theme configurations for the active business context.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\UserProfileThemesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->usersGetMyTheme();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserProfileThemesApi->usersGetMyTheme: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\Solifyn\Model\UserTheme**](../Model/UserTheme.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `usersGetSettings()`

```php
usersGetSettings(): \Solifyn\Model\UserSettings
```

Retrieve User Settings

Retrieve profile settings and notification preferences for the user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\UserProfileThemesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->usersGetSettings();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserProfileThemesApi->usersGetSettings: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\Solifyn\Model\UserSettings**](../Model/UserSettings.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `usersGetStats()`

```php
usersGetStats(): \Solifyn\Model\UserStats
```

Get Dashboard Statistics

Retrieve general analytics stats (revenue, order counts, etc.) for dashboard graphs.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\UserProfileThemesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->usersGetStats();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserProfileThemesApi->usersGetStats: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\Solifyn\Model\UserStats**](../Model/UserStats.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `usersGetThemeBySubdomain()`

```php
usersGetThemeBySubdomain($subdomain): \Solifyn\Model\UserTheme
```

Get Theme by Subdomain

Retrieve public theme configuration details by store subdomain.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\UserProfileThemesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$subdomain = acme; // string | The subdomain of the store

try {
    $result = $apiInstance->usersGetThemeBySubdomain($subdomain);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserProfileThemesApi->usersGetThemeBySubdomain: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subdomain** | **string**| The subdomain of the store | |

### Return type

[**\Solifyn\Model\UserTheme**](../Model/UserTheme.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
