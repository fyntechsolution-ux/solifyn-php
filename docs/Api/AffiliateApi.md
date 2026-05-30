# Solifyn\AffiliateApi

All URIs are relative to http://localhost:8000, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**affiliateControllerApproveConnection()**](AffiliateApi.md#affiliateControllerApproveConnection) | **POST** /v1/affiliate/program/connections/{id}/approve |  |
| [**affiliateControllerArchiveConnection()**](AffiliateApi.md#affiliateControllerArchiveConnection) | **POST** /v1/affiliate/program/connections/{id}/archive |  |
| [**affiliateControllerDeleteOverride()**](AffiliateApi.md#affiliateControllerDeleteOverride) | **DELETE** /v1/affiliate/program/override/{id} |  |
| [**affiliateControllerGetEarningsConnections()**](AffiliateApi.md#affiliateControllerGetEarningsConnections) | **GET** /v1/affiliate/earnings/connections |  |
| [**affiliateControllerGetEarningsLedger()**](AffiliateApi.md#affiliateControllerGetEarningsLedger) | **GET** /v1/affiliate/earnings/ledger |  |
| [**affiliateControllerGetEarningsStats()**](AffiliateApi.md#affiliateControllerGetEarningsStats) | **GET** /v1/affiliate/earnings/stats |  |
| [**affiliateControllerGetMarketplace()**](AffiliateApi.md#affiliateControllerGetMarketplace) | **GET** /v1/affiliate/marketplace |  |
| [**affiliateControllerGetProgramConnections()**](AffiliateApi.md#affiliateControllerGetProgramConnections) | **GET** /v1/affiliate/program/connections |  |
| [**affiliateControllerGetProgramLedger()**](AffiliateApi.md#affiliateControllerGetProgramLedger) | **GET** /v1/affiliate/program/ledger |  |
| [**affiliateControllerGetProgramSettings()**](AffiliateApi.md#affiliateControllerGetProgramSettings) | **GET** /v1/affiliate/program/settings |  |
| [**affiliateControllerJoinProgram()**](AffiliateApi.md#affiliateControllerJoinProgram) | **POST** /v1/affiliate/marketplace/join |  |
| [**affiliateControllerRejectConnection()**](AffiliateApi.md#affiliateControllerRejectConnection) | **POST** /v1/affiliate/program/connections/{id}/reject |  |
| [**affiliateControllerSaveOverride()**](AffiliateApi.md#affiliateControllerSaveOverride) | **POST** /v1/affiliate/program/override |  |
| [**affiliateControllerSaveProgramSettings()**](AffiliateApi.md#affiliateControllerSaveProgramSettings) | **POST** /v1/affiliate/program/settings |  |


## `affiliateControllerApproveConnection()`

```php
affiliateControllerApproveConnection($id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 'id_example'; // string

try {
    $apiInstance->affiliateControllerApproveConnection($id);
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerApproveConnection: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerArchiveConnection()`

```php
affiliateControllerArchiveConnection($id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 'id_example'; // string

try {
    $apiInstance->affiliateControllerArchiveConnection($id);
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerArchiveConnection: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerDeleteOverride()`

```php
affiliateControllerDeleteOverride($id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 'id_example'; // string

try {
    $apiInstance->affiliateControllerDeleteOverride($id);
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerDeleteOverride: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerGetEarningsConnections()`

```php
affiliateControllerGetEarningsConnections()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->affiliateControllerGetEarningsConnections();
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerGetEarningsConnections: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerGetEarningsLedger()`

```php
affiliateControllerGetEarningsLedger()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->affiliateControllerGetEarningsLedger();
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerGetEarningsLedger: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerGetEarningsStats()`

```php
affiliateControllerGetEarningsStats()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->affiliateControllerGetEarningsStats();
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerGetEarningsStats: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerGetMarketplace()`

```php
affiliateControllerGetMarketplace()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->affiliateControllerGetMarketplace();
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerGetMarketplace: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerGetProgramConnections()`

```php
affiliateControllerGetProgramConnections()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->affiliateControllerGetProgramConnections();
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerGetProgramConnections: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerGetProgramLedger()`

```php
affiliateControllerGetProgramLedger()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->affiliateControllerGetProgramLedger();
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerGetProgramLedger: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerGetProgramSettings()`

```php
affiliateControllerGetProgramSettings()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->affiliateControllerGetProgramSettings();
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerGetProgramSettings: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerJoinProgram()`

```php
affiliateControllerJoinProgram()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->affiliateControllerJoinProgram();
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerJoinProgram: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerRejectConnection()`

```php
affiliateControllerRejectConnection($id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 'id_example'; // string

try {
    $apiInstance->affiliateControllerRejectConnection($id);
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerRejectConnection: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerSaveOverride()`

```php
affiliateControllerSaveOverride()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->affiliateControllerSaveOverride();
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerSaveOverride: ', $e->getMessage(), PHP_EOL;
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

## `affiliateControllerSaveProgramSettings()`

```php
affiliateControllerSaveProgramSettings()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\AffiliateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->affiliateControllerSaveProgramSettings();
} catch (Exception $e) {
    echo 'Exception when calling AffiliateApi->affiliateControllerSaveProgramSettings: ', $e->getMessage(), PHP_EOL;
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
