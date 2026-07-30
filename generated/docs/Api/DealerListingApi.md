# ShadowSoftware\Sdk\Generated\DealerListingApi



All URIs are relative to http://localhost:8080/api/v1/dealer, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**dealerApiListingsDestroy()**](DealerListingApi.md#dealerApiListingsDestroy) | **DELETE** /listings/{urlSlug} | Soft-delete. Reversible: the images survive, so restore() brings the listing back whole. Trashing a product in WooCommerce lands here |
| [**dealerApiListingsIndex()**](DealerListingApi.md#dealerApiListingsIndex) | **GET** /listings | The dealer&#39;s listings, newest first |
| [**dealerApiListingsRestore()**](DealerListingApi.md#dealerApiListingsRestore) | **POST** /listings/{urlSlug}/restore | Un-delete. Restoring a product from the WooCommerce trash lands here, which is what makes the two sides symmetrical |
| [**dealerApiListingsShow()**](DealerListingApi.md#dealerApiListingsShow) | **GET** /listings/{urlSlug} |  |
| [**dealerApiListingsStatus()**](DealerListingApi.md#dealerApiListingsStatus) | **GET** /listings/status | Bulk status poll — the AGT-to-WooCommerce writeback channel |
| [**dealerApiListingsStore()**](DealerListingApi.md#dealerApiListingsStore) | **POST** /listings |  |
| [**dealerApiListingsUpdate()**](DealerListingApi.md#dealerApiListingsUpdate) | **PUT** /listings/{urlSlug} |  |


## `dealerApiListingsDestroy()`

```php
dealerApiListingsDestroy($url_slug): \ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStore201Response
```

Soft-delete. Reversible: the images survive, so restore() brings the listing back whole. Trashing a product in WooCommerce lands here

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new ShadowSoftware\Sdk\Generated\Api\DealerListingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$url_slug = 'url_slug_example'; // string

try {
    $result = $apiInstance->dealerApiListingsDestroy($url_slug);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DealerListingApi->dealerApiListingsDestroy: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **url_slug** | **string**|  | |

### Return type

[**\ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStore201Response**](../Model/DealerApiListingsStore201Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `dealerApiListingsIndex()`

```php
dealerApiListingsIndex(): \ShadowSoftware\Sdk\Generated\Model\DealerApiListingsIndex200Response
```

The dealer's listings, newest first

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new ShadowSoftware\Sdk\Generated\Api\DealerListingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->dealerApiListingsIndex();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DealerListingApi->dealerApiListingsIndex: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\ShadowSoftware\Sdk\Generated\Model\DealerApiListingsIndex200Response**](../Model/DealerApiListingsIndex200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `dealerApiListingsRestore()`

```php
dealerApiListingsRestore($url_slug): \ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStore201Response
```

Un-delete. Restoring a product from the WooCommerce trash lands here, which is what makes the two sides symmetrical

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new ShadowSoftware\Sdk\Generated\Api\DealerListingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$url_slug = 'url_slug_example'; // string

try {
    $result = $apiInstance->dealerApiListingsRestore($url_slug);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DealerListingApi->dealerApiListingsRestore: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **url_slug** | **string**|  | |

### Return type

[**\ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStore201Response**](../Model/DealerApiListingsStore201Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `dealerApiListingsShow()`

```php
dealerApiListingsShow($url_slug): \ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStore201Response
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new ShadowSoftware\Sdk\Generated\Api\DealerListingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$url_slug = 'url_slug_example'; // string

try {
    $result = $apiInstance->dealerApiListingsShow($url_slug);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DealerListingApi->dealerApiListingsShow: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **url_slug** | **string**|  | |

### Return type

[**\ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStore201Response**](../Model/DealerApiListingsStore201Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `dealerApiListingsStatus()`

```php
dealerApiListingsStatus(): \ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStatus200Response
```

Bulk status poll — the AGT-to-WooCommerce writeback channel

The plugin calls this on a schedule with the slugs it knows about and gets back one small object per listing. This is what turns \"it sold on AGT\" into \"the WooCommerce product is out of stock\" without AGT ever having to reach into the dealer's store, which is exactly what most dealer sites (behind a WAF, on a private host) could not accept anyway.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new ShadowSoftware\Sdk\Generated\Api\DealerListingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->dealerApiListingsStatus();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DealerListingApi->dealerApiListingsStatus: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStatus200Response**](../Model/DealerApiListingsStatus200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `dealerApiListingsStore()`

```php
dealerApiListingsStore($title, $description, $price, $condition, $category_id, $images, $manufacturer_id, $caliber_id, $weight, $applications): \ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStore201Response
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new ShadowSoftware\Sdk\Generated\Api\DealerListingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$title = 'title_example'; // string
$description = 'description_example'; // string
$price = 3.4; // float
$condition = 56; // int
$category_id = 56; // int
$images = array('/path/to/file.txt'); // \SplFileObject[]
$manufacturer_id = 56; // int
$caliber_id = 56; // int
$weight = 3.4; // float
$applications = array(56); // int[]

try {
    $result = $apiInstance->dealerApiListingsStore($title, $description, $price, $condition, $category_id, $images, $manufacturer_id, $caliber_id, $weight, $applications);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DealerListingApi->dealerApiListingsStore: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **title** | **string**|  | |
| **description** | **string**|  | |
| **price** | **float**|  | |
| **condition** | **int**|  | |
| **category_id** | **int**|  | |
| **images** | **\SplFileObject[]**|  | |
| **manufacturer_id** | **int**|  | [optional] |
| **caliber_id** | **int**|  | [optional] |
| **weight** | **float**|  | [optional] |
| **applications** | [**int[]**](../Model/int.md)|  | [optional] |

### Return type

[**\ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStore201Response**](../Model/DealerApiListingsStore201Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `dealerApiListingsUpdate()`

```php
dealerApiListingsUpdate($url_slug, $title, $description, $price, $condition, $category_id, $manufacturer_id, $caliber_id, $weight, $applications, $images): \ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStore201Response
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new ShadowSoftware\Sdk\Generated\Api\DealerListingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$url_slug = 'url_slug_example'; // string
$title = 'title_example'; // string
$description = 'description_example'; // string
$price = 3.4; // float
$condition = 56; // int
$category_id = 56; // int
$manufacturer_id = 56; // int
$caliber_id = 56; // int
$weight = 3.4; // float
$applications = array(56); // int[]
$images = array('/path/to/file.txt'); // \SplFileObject[] | Sending images replaces the whole set — WooCommerce owns the gallery.

try {
    $result = $apiInstance->dealerApiListingsUpdate($url_slug, $title, $description, $price, $condition, $category_id, $manufacturer_id, $caliber_id, $weight, $applications, $images);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DealerListingApi->dealerApiListingsUpdate: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **url_slug** | **string**|  | |
| **title** | **string**|  | [optional] |
| **description** | **string**|  | [optional] |
| **price** | **float**|  | [optional] |
| **condition** | **int**|  | [optional] |
| **category_id** | **int**|  | [optional] |
| **manufacturer_id** | **int**|  | [optional] |
| **caliber_id** | **int**|  | [optional] |
| **weight** | **float**|  | [optional] |
| **applications** | [**int[]**](../Model/int.md)|  | [optional] |
| **images** | **\SplFileObject[]**| Sending images replaces the whole set — WooCommerce owns the gallery. | [optional] |

### Return type

[**\ShadowSoftware\Sdk\Generated\Model\DealerApiListingsStore201Response**](../Model/DealerApiListingsStore201Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
