# MehrIt\OttoQuantitiesApiClient\AvailableQuantityApi

All URIs are relative to *https://available-quantity-gateway.develop.availability.platform.otto.de/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**storeAvailableQuantitiesUsingPOST**](AvailableQuantityApi.md#storeavailablequantitiesusingpost) | **POST** /v2/quantities | Update the available quantity for a specific SKU (up to 200 SKUs per request)

# **storeAvailableQuantitiesUsingPOST**
> object storeAvailableQuantitiesUsingPOST($body)

Update the available quantity for a specific SKU (up to 200 SKUs per request)

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new MehrIt\OttoQuantitiesApiClient\Api\AvailableQuantityApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = array(new \MehrIt\OttoQuantitiesApiClient\Model\AvailableQuantityRequestDTOV2()); // \MehrIt\OttoQuantitiesApiClient\Model\AvailableQuantityRequestDTOV2[] | availableQuantityRequestDTO

try {
    $result = $apiInstance->storeAvailableQuantitiesUsingPOST($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AvailableQuantityApi->storeAvailableQuantitiesUsingPOST: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\MehrIt\OttoQuantitiesApiClient\Model\AvailableQuantityRequestDTOV2[]**](../Model/AvailableQuantityRequestDTOV2.md)| availableQuantityRequestDTO |

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json;charset=UTF-8
 - **Accept**: application/json;charset=UTF-8

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

