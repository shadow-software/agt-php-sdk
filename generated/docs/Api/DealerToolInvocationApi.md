# ShadowSoftware\Agt\DealerToolInvocationApi



All URIs are relative to http://localhost:8080/api/v1/dealer, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**dealerApiToolsInvoke()**](DealerToolInvocationApi.md#dealerApiToolsInvoke) | **POST** /tools/{tool} |  |


## `dealerApiToolsInvoke()`

```php
dealerApiToolsInvoke($tool): \ShadowSoftware\Agt\Model\DealerApiToolsInvoke200Response
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new ShadowSoftware\Agt\Api\DealerToolInvocationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$tool = 'tool_example'; // string

try {
    $result = $apiInstance->dealerApiToolsInvoke($tool);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DealerToolInvocationApi->dealerApiToolsInvoke: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tool** | **string**|  | |

### Return type

[**\ShadowSoftware\Agt\Model\DealerApiToolsInvoke200Response**](../Model/DealerApiToolsInvoke200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
