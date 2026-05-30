# Solifyn\BrandsApi

All URIs are relative to http://localhost:8000, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**brandsCreate()**](BrandsApi.md#brandsCreate) | **POST** /v1/user/brand | Create Brand |
| [**brandsGet()**](BrandsApi.md#brandsGet) | **GET** /v1/user/brand/{id} | Retrieve Brand |
| [**brandsList()**](BrandsApi.md#brandsList) | **GET** /v1/user/brands | List Brands |
| [**brandsUpdate()**](BrandsApi.md#brandsUpdate) | **PATCH** /v1/user/brand/{id} | Update Brand |


## `brandsCreate()`

```php
brandsCreate($brand_create): \Solifyn\Model\Brand
```

Create Brand

Add a new brand identity under the current active business.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\BrandsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$brand_create = new \Solifyn\Model\BrandCreate(); // \Solifyn\Model\BrandCreate

try {
    $result = $apiInstance->brandsCreate($brand_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandsApi->brandsCreate: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **brand_create** | [**\Solifyn\Model\BrandCreate**](../Model/BrandCreate.md)|  | |

### Return type

[**\Solifyn\Model\Brand**](../Model/Brand.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `brandsGet()`

```php
brandsGet($id): \Solifyn\Model\Brand
```

Retrieve Brand

Retrieve details of a brand identity by ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\BrandsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = brd_123; // string | The brand ID to retrieve

try {
    $result = $apiInstance->brandsGet($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandsApi->brandsGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The brand ID to retrieve | |

### Return type

[**\Solifyn\Model\Brand**](../Model/Brand.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `brandsList()`

```php
brandsList(): \Solifyn\Model\Brand[]
```

List Brands

Retrieve all brands associated with the current business context.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\BrandsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->brandsList();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandsApi->brandsList: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\Solifyn\Model\Brand[]**](../Model/Brand.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `brandsUpdate()`

```php
brandsUpdate($id, $brand_update): \Solifyn\Model\Brand
```

Update Brand

Update website, logo, description, or statement descriptors of a brand.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\BrandsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = brd_123; // string | The brand ID to update
$brand_update = new \Solifyn\Model\BrandUpdate(); // \Solifyn\Model\BrandUpdate

try {
    $result = $apiInstance->brandsUpdate($id, $brand_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandsApi->brandsUpdate: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The brand ID to update | |
| **brand_update** | [**\Solifyn\Model\BrandUpdate**](../Model/BrandUpdate.md)|  | |

### Return type

[**\Solifyn\Model\Brand**](../Model/Brand.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
