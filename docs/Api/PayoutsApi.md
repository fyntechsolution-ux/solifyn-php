# Solifyn\PayoutsApi

All URIs are relative to http://localhost:8000, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**payoutsCreateWithdrawal()**](PayoutsApi.md#payoutsCreateWithdrawal) | **POST** /v1/payouts/withdrawals | Create Withdrawal |
| [**payoutsGetAccount()**](PayoutsApi.md#payoutsGetAccount) | **GET** /v1/payouts/account | Retrieve Payout Account |
| [**payoutsGetAccountLink()**](PayoutsApi.md#payoutsGetAccountLink) | **GET** /v1/payouts/account-link | Create Account Link |
| [**payoutsGetToken()**](PayoutsApi.md#payoutsGetToken) | **GET** /v1/payouts/token | Generate Portal Access Token |
| [**payoutsGetWithdrawals()**](PayoutsApi.md#payoutsGetWithdrawals) | **GET** /v1/payouts/withdrawals | Get Withdrawals List |
| [**payoutsListMethods()**](PayoutsApi.md#payoutsListMethods) | **GET** /v1/payouts/methods | List Payout Methods |
| [**payoutsListVerifications()**](PayoutsApi.md#payoutsListVerifications) | **GET** /v1/payouts/verifications | List Verifications |
| [**payoutsListWithdrawals()**](PayoutsApi.md#payoutsListWithdrawals) | **GET** /v1/payouts | List Withdrawals |


## `payoutsCreateWithdrawal()`

```php
payoutsCreateWithdrawal($withdrawal_create): \Solifyn\Model\Withdrawal
```

Create Withdrawal

Initiate a balance withdrawal transfer request.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\PayoutsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$withdrawal_create = new \Solifyn\Model\WithdrawalCreate(); // \Solifyn\Model\WithdrawalCreate

try {
    $result = $apiInstance->payoutsCreateWithdrawal($withdrawal_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PayoutsApi->payoutsCreateWithdrawal: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **withdrawal_create** | [**\Solifyn\Model\WithdrawalCreate**](../Model/WithdrawalCreate.md)|  | |

### Return type

[**\Solifyn\Model\Withdrawal**](../Model/Withdrawal.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `payoutsGetAccount()`

```php
payoutsGetAccount(): \Solifyn\Model\PayoutAccount
```

Retrieve Payout Account

Retrieve general status and information of onboarding payout accounts.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\PayoutsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->payoutsGetAccount();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PayoutsApi->payoutsGetAccount: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\Solifyn\Model\PayoutAccount**](../Model/PayoutAccount.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `payoutsGetAccountLink()`

```php
payoutsGetAccountLink($use_case): \Solifyn\Model\PayoutAccountLink
```

Create Account Link

Generate temporary links for onboarding or viewing portals.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\PayoutsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$use_case = 'use_case_example'; // string | Onboarding link type context

try {
    $result = $apiInstance->payoutsGetAccountLink($use_case);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PayoutsApi->payoutsGetAccountLink: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **use_case** | **string**| Onboarding link type context | [optional] |

### Return type

[**\Solifyn\Model\PayoutAccountLink**](../Model/PayoutAccountLink.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `payoutsGetToken()`

```php
payoutsGetToken(): \Solifyn\Model\PayoutAccessToken
```

Generate Portal Access Token

Generate temporary credentials to access the embed portal.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\PayoutsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->payoutsGetToken();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PayoutsApi->payoutsGetToken: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\Solifyn\Model\PayoutAccessToken**](../Model/PayoutAccessToken.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `payoutsGetWithdrawals()`

```php
payoutsGetWithdrawals($limit, $page): \Solifyn\Model\WithdrawalList
```

Get Withdrawals List

Retrieve withdrawal records for the active business.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\PayoutsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$limit = 3.4; // float | Page size limit
$page = 3.4; // float | Page number

try {
    $result = $apiInstance->payoutsGetWithdrawals($limit, $page);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PayoutsApi->payoutsGetWithdrawals: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **float**| Page size limit | [optional] |
| **page** | **float**| Page number | [optional] |

### Return type

[**\Solifyn\Model\WithdrawalList**](../Model/WithdrawalList.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `payoutsListMethods()`

```php
payoutsListMethods($limit, $page): \Solifyn\Model\PayoutMethodList
```

List Payout Methods

List saved payout destinations (bank accounts, cards).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\PayoutsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$limit = 3.4; // float
$page = 3.4; // float

try {
    $result = $apiInstance->payoutsListMethods($limit, $page);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PayoutsApi->payoutsListMethods: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **float**|  | [optional] |
| **page** | **float**|  | [optional] |

### Return type

[**\Solifyn\Model\PayoutMethodList**](../Model/PayoutMethodList.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `payoutsListVerifications()`

```php
payoutsListVerifications($limit, $page): \Solifyn\Model\PayoutVerificationList
```

List Verifications

Retrieve pending or completed KYC verification checks.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\PayoutsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$limit = 3.4; // float
$page = 3.4; // float

try {
    $result = $apiInstance->payoutsListVerifications($limit, $page);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PayoutsApi->payoutsListVerifications: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **float**|  | [optional] |
| **page** | **float**|  | [optional] |

### Return type

[**\Solifyn\Model\PayoutVerificationList**](../Model/PayoutVerificationList.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `payoutsListWithdrawals()`

```php
payoutsListWithdrawals($limit, $page): \Solifyn\Model\WithdrawalList
```

List Withdrawals

Retrieve a list of past withdrawal history.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (API Key) authorization: ApiKeyAuth
$config = Solifyn\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Solifyn\Api\PayoutsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$limit = 3.4; // float | Page size limit
$page = 3.4; // float | Page number

try {
    $result = $apiInstance->payoutsListWithdrawals($limit, $page);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PayoutsApi->payoutsListWithdrawals: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **float**| Page size limit | [optional] |
| **page** | **float**| Page number | [optional] |

### Return type

[**\Solifyn\Model\WithdrawalList**](../Model/WithdrawalList.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
