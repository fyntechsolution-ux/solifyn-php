# Solifyn\ChatApi

All URIs are relative to http://localhost:8000, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatControllerGetMerchantMessages()**](ChatApi.md#chatControllerGetMerchantMessages) | **GET** /v1/chat/merchant/messages/{customerId} |  |
| [**chatControllerGetMerchantSessions()**](ChatApi.md#chatControllerGetMerchantSessions) | **GET** /v1/chat/merchant/sessions |  |
| [**chatControllerSendCustomerMessage()**](ChatApi.md#chatControllerSendCustomerMessage) | **POST** /v1/chat/customer/message |  |
| [**chatControllerSendMerchantMessage()**](ChatApi.md#chatControllerSendMerchantMessage) | **POST** /v1/chat/merchant/message |  |


## `chatControllerGetMerchantMessages()`

```php
chatControllerGetMerchantMessages($customer_id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\ChatApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$customer_id = 'customer_id_example'; // string

try {
    $apiInstance->chatControllerGetMerchantMessages($customer_id);
} catch (Exception $e) {
    echo 'Exception when calling ChatApi->chatControllerGetMerchantMessages: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customer_id** | **string**|  | |

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

## `chatControllerGetMerchantSessions()`

```php
chatControllerGetMerchantSessions()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\ChatApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->chatControllerGetMerchantSessions();
} catch (Exception $e) {
    echo 'Exception when calling ChatApi->chatControllerGetMerchantSessions: ', $e->getMessage(), PHP_EOL;
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

## `chatControllerSendCustomerMessage()`

```php
chatControllerSendCustomerMessage()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\ChatApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->chatControllerSendCustomerMessage();
} catch (Exception $e) {
    echo 'Exception when calling ChatApi->chatControllerSendCustomerMessage: ', $e->getMessage(), PHP_EOL;
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

## `chatControllerSendMerchantMessage()`

```php
chatControllerSendMerchantMessage()
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new Solifyn\Api\ChatApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->chatControllerSendMerchantMessage();
} catch (Exception $e) {
    echo 'Exception when calling ChatApi->chatControllerSendMerchantMessage: ', $e->getMessage(), PHP_EOL;
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
