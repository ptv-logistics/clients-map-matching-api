# PositionsApi

All URIs are relative to *https://api.myptv.com/mapmatch/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**matchPosition**](PositionsApi.md#matchposition) | **GET** /positions/{latitude}/{longitude} |  |



## matchPosition

> MatchedPosition matchPosition(latitude, longitude, heading, calculationMode, results, language)



Matches a single unrelated position on a map.

### Example

```ts
import {
  Configuration,
  PositionsApi,
} from '';
import type { MatchPositionRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new PositionsApi(config);

  const body = {
    // number
    latitude: 49.480301,
    // number
    longitude: 6.110667,
    // number | The direction of travel defined by a clockwise angle with respect to north in degrees \\[°\\], e.g., 0° is north, 90° is east, 180° is south, and 270° is west. Specifying the **heading** will improve the quality of the results. (optional)
    heading: 10,
    // CalculationMode | The calculationMode affects the quality and performance of the matching. (optional)
    calculationMode: ...,
    // Array<PositionsResultType> | Selects which properties the MatchedPosition will contain. (optional)
    results: ...,
    // string | The preferred language for the response formatted according to [ISO-639-1](https://www.loc.gov/standards/iso639-2/php/code_list.php) for languages or [BCP47](https://tools.ietf.org/html/bcp47) for language variants. By default the service uses the language spoken in the country or region of the result. In case the given preferred language is not available in the data, the default language is used. (optional)
    language: en,
  } satisfies MatchPositionRequest;

  try {
    const data = await api.matchPosition(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **latitude** | `number` |  | [Defaults to `undefined`] |
| **longitude** | `number` |  | [Defaults to `undefined`] |
| **heading** | `number` | The direction of travel defined by a clockwise angle with respect to north in degrees \\[°\\], e.g., 0° is north, 90° is east, 180° is south, and 270° is west. Specifying the **heading** will improve the quality of the results. | [Optional] [Defaults to `undefined`] |
| **calculationMode** | `CalculationMode` | The calculationMode affects the quality and performance of the matching. | [Optional] [Defaults to `undefined`] [Enum: PERFORMANCE, STANDARD, QUALITY] |
| **results** | `Array<PositionsResultType>` | Selects which properties the MatchedPosition will contain. | [Optional] |
| **language** | `string` | The preferred language for the response formatted according to [ISO-639-1](https://www.loc.gov/standards/iso639-2/php/code_list.php) for languages or [BCP47](https://tools.ietf.org/html/bcp47) for language variants. By default the service uses the language spoken in the country or region of the result. In case the given preferred language is not available in the data, the default language is used. | [Optional] [Defaults to `undefined`] |

### Return type

[**MatchedPosition**](MatchedPosition.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Response on success. |  -  |
| **0** | Response on failure. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

