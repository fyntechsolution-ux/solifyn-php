# Solifyn\PartnerApi

All URIs are relative to http://localhost:8000, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**partnerControllerGetPartnerCommissions()**](PartnerApi.md#partnerControllerGetPartnerCommissions) | **GET** /v1/partner/commissions |  |
| [**partnerControllerGetPartnerStats()**](PartnerApi.md#partnerControllerGetPartnerStats) | **GET** /v1/partner/stats |  |


## `partnerControllerGetPartnerCommissions()`

```php
partnerControllerGetPartnerCommissions()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->partnerControllerGetPartnerCommissions();
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->partnerControllerGetPartnerCommissions: ', $e->getMessage(), PHP_EOL;
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

## `partnerControllerGetPartnerStats()`

```php
partnerControllerGetPartnerStats()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->partnerControllerGetPartnerStats();
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->partnerControllerGetPartnerStats: ', $e->getMessage(), PHP_EOL;
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
