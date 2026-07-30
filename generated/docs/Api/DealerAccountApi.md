# ShadowSoftware\Agt\DealerAccountApi



All URIs are relative to http://localhost:8080/api/v1/dealer, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**dealerApiMe()**](DealerAccountApi.md#dealerApiMe) | **GET** /me | The dealer&#39;s identity and, crucially, whether they can publish right now |
| [**dealerApiTaxonomy()**](DealerAccountApi.md#dealerApiTaxonomy) | **GET** /taxonomy | Everything the plugin needs to build a valid listing: the category tree, the manufacturers, the calibers, the applications, and the conditions |


## `dealerApiMe()`

```php
dealerApiMe(): \ShadowSoftware\Agt\Model\DealerApiMe200Response
```

The dealer's identity and, crucially, whether they can publish right now

`can_publish` is the single flag the plugin gates on. If it is false the plugin must stop and show `blockers` rather than firing a catalog of doomed requests at a 409.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new ShadowSoftware\Agt\Api\DealerAccountApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->dealerApiMe();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DealerAccountApi->dealerApiMe: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\ShadowSoftware\Agt\Model\DealerApiMe200Response**](../Model/DealerApiMe200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `dealerApiTaxonomy()`

```php
dealerApiTaxonomy(): \ShadowSoftware\Agt\Model\DealerApiTaxonomy200Response
```

Everything the plugin needs to build a valid listing: the category tree, the manufacturers, the calibers, the applications, and the conditions

Cached and ETagged — the plugin refreshes it daily, and a store with an unchanged copy gets a 304 rather than a payload.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new ShadowSoftware\Agt\Api\DealerAccountApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->dealerApiTaxonomy();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DealerAccountApi->dealerApiTaxonomy: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\ShadowSoftware\Agt\Model\DealerApiTaxonomy200Response**](../Model/DealerApiTaxonomy200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
