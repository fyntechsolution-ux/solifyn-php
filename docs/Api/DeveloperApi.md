# Solifyn\DeveloperApi

All URIs are relative to http://localhost:8000, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**developerControllerCreateApiKey()**](DeveloperApi.md#developerControllerCreateApiKey) | **POST** /v1/developer/api-keys |  |
| [**developerControllerCreateWebhookEndpoint()**](DeveloperApi.md#developerControllerCreateWebhookEndpoint) | **POST** /v1/developer/webhooks |  |
| [**developerControllerDeleteApiKey()**](DeveloperApi.md#developerControllerDeleteApiKey) | **DELETE** /v1/developer/api-keys/{id} |  |
| [**developerControllerDeleteWebhookEndpoint()**](DeveloperApi.md#developerControllerDeleteWebhookEndpoint) | **DELETE** /v1/developer/webhooks/{id} |  |
| [**developerControllerGetApiKeys()**](DeveloperApi.md#developerControllerGetApiKeys) | **GET** /v1/developer/api-keys |  |
| [**developerControllerGetAppPortalUrl()**](DeveloperApi.md#developerControllerGetAppPortalUrl) | **GET** /v1/developer/webhooks/app-portal |  |
| [**developerControllerGetWebhookDeliveries()**](DeveloperApi.md#developerControllerGetWebhookDeliveries) | **GET** /v1/developer/webhooks/{id}/deliveries |  |
| [**developerControllerGetWebhookEndpoints()**](DeveloperApi.md#developerControllerGetWebhookEndpoints) | **GET** /v1/developer/webhooks |  |
| [**developerControllerUpdateWebhookEndpoint()**](DeveloperApi.md#developerControllerUpdateWebhookEndpoint) | **PATCH** /v1/developer/webhooks/{id} |  |


## `developerControllerCreateApiKey()`

```php
developerControllerCreateApiKey()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\DeveloperApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->developerControllerCreateApiKey();
} catch (Exception $e) {
    echo 'Exception when calling DeveloperApi->developerControllerCreateApiKey: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `developerControllerCreateWebhookEndpoint()`

```php
developerControllerCreateWebhookEndpoint()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\DeveloperApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->developerControllerCreateWebhookEndpoint();
} catch (Exception $e) {
    echo 'Exception when calling DeveloperApi->developerControllerCreateWebhookEndpoint: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `developerControllerDeleteApiKey()`

```php
developerControllerDeleteApiKey($id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\DeveloperApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 'id_example'; // string

try {
    $apiInstance->developerControllerDeleteApiKey($id);
} catch (Exception $e) {
    echo 'Exception when calling DeveloperApi->developerControllerDeleteApiKey: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `developerControllerDeleteWebhookEndpoint()`

```php
developerControllerDeleteWebhookEndpoint($id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\DeveloperApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 'id_example'; // string

try {
    $apiInstance->developerControllerDeleteWebhookEndpoint($id);
} catch (Exception $e) {
    echo 'Exception when calling DeveloperApi->developerControllerDeleteWebhookEndpoint: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `developerControllerGetApiKeys()`

```php
developerControllerGetApiKeys()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\DeveloperApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->developerControllerGetApiKeys();
} catch (Exception $e) {
    echo 'Exception when calling DeveloperApi->developerControllerGetApiKeys: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `developerControllerGetAppPortalUrl()`

```php
developerControllerGetAppPortalUrl()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\DeveloperApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->developerControllerGetAppPortalUrl();
} catch (Exception $e) {
    echo 'Exception when calling DeveloperApi->developerControllerGetAppPortalUrl: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `developerControllerGetWebhookDeliveries()`

```php
developerControllerGetWebhookDeliveries($id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\DeveloperApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 'id_example'; // string

try {
    $apiInstance->developerControllerGetWebhookDeliveries($id);
} catch (Exception $e) {
    echo 'Exception when calling DeveloperApi->developerControllerGetWebhookDeliveries: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `developerControllerGetWebhookEndpoints()`

```php
developerControllerGetWebhookEndpoints()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\DeveloperApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->developerControllerGetWebhookEndpoints();
} catch (Exception $e) {
    echo 'Exception when calling DeveloperApi->developerControllerGetWebhookEndpoints: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `developerControllerUpdateWebhookEndpoint()`

```php
developerControllerUpdateWebhookEndpoint($id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\DeveloperApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 'id_example'; // string

try {
    $apiInstance->developerControllerUpdateWebhookEndpoint($id);
} catch (Exception $e) {
    echo 'Exception when calling DeveloperApi->developerControllerUpdateWebhookEndpoint: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
