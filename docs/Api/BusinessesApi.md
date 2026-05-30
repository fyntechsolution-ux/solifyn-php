# Solifyn\BusinessesApi

All URIs are relative to http://localhost:8000, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**businessesBillingHistory()**](BusinessesApi.md#businessesBillingHistory) | **GET** /v1/user/billing/history | Get Platform Billing History |
| [**merchantsGenerateApiKeys()**](BusinessesApi.md#merchantsGenerateApiKeys) | **POST** /v1/user/whop-api-keys | Rotate Whop API Keys |
| [**merchantsUpdatePage()**](BusinessesApi.md#merchantsUpdatePage) | **PATCH** /v1/user/page | Update Page configuration |
| [**merchantsUpdateSettings()**](BusinessesApi.md#merchantsUpdateSettings) | **PATCH** /v1/user/settings | Update Merchant Settings |
| [**merchantsUpdateTheme()**](BusinessesApi.md#merchantsUpdateTheme) | **PATCH** /v1/user/theme | Update Theme |


## `businessesBillingHistory()`

```php
businessesBillingHistory()
```

Get Platform Billing History

Retrieve history of SaaS subscription payments paid by this business to the platform.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\BusinessesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $apiInstance->businessesBillingHistory();
} catch (Exception $e) {
    echo 'Exception when calling BusinessesApi->businessesBillingHistory: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `merchantsGenerateApiKeys()`

```php
merchantsGenerateApiKeys(): \Solifyn\Model\WhopApiKeysRotation
```

Rotate Whop API Keys

Generate and sync a new Whop Child Company API key (restricted to business owners).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\BusinessesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->merchantsGenerateApiKeys();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BusinessesApi->merchantsGenerateApiKeys: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\Solifyn\Model\WhopApiKeysRotation**](../Model/WhopApiKeysRotation.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `merchantsUpdatePage()`

```php
merchantsUpdatePage($user_theme_update): \Solifyn\Model\UserPage
```

Update Page configuration

Modify store page content configs, banner images, or avatar details.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\BusinessesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$user_theme_update = new \Solifyn\Model\UserThemeUpdate(); // \Solifyn\Model\UserThemeUpdate

try {
    $result = $apiInstance->merchantsUpdatePage($user_theme_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BusinessesApi->merchantsUpdatePage: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_theme_update** | [**\Solifyn\Model\UserThemeUpdate**](../Model/UserThemeUpdate.md)|  | |

### Return type

[**\Solifyn\Model\UserPage**](../Model/UserPage.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `merchantsUpdateSettings()`

```php
merchantsUpdateSettings($user_settings_update): \Solifyn\Model\UserSettings
```

Update Merchant Settings

Update profile parameters, SEO, Google analytics, and email notification properties.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\BusinessesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$user_settings_update = new \Solifyn\Model\UserSettingsUpdate(); // \Solifyn\Model\UserSettingsUpdate

try {
    $result = $apiInstance->merchantsUpdateSettings($user_settings_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BusinessesApi->merchantsUpdateSettings: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_settings_update** | [**\Solifyn\Model\UserSettingsUpdate**](../Model/UserSettingsUpdate.md)|  | |

### Return type

[**\Solifyn\Model\UserSettings**](../Model/UserSettings.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `merchantsUpdateTheme()`

```php
merchantsUpdateTheme($user_theme_update): \Solifyn\Model\UserTheme
```

Update Theme

Update colors, fonts, avatar, or banner settings for the store.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\BusinessesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$user_theme_update = new \Solifyn\Model\UserThemeUpdate(); // \Solifyn\Model\UserThemeUpdate

try {
    $result = $apiInstance->merchantsUpdateTheme($user_theme_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BusinessesApi->merchantsUpdateTheme: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_theme_update** | [**\Solifyn\Model\UserThemeUpdate**](../Model/UserThemeUpdate.md)|  | |

### Return type

[**\Solifyn\Model\UserTheme**](../Model/UserTheme.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
