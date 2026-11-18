# TracksApi

All URIs are relative to *https://api.myptv.com/mapmatch/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createMatchedTrack**](TracksApi.md#creatematchedtrack) | **POST** /tracks |  |
| [**deleteMatchedTrack**](TracksApi.md#deletematchedtrack) | **DELETE** /tracks/{id} |  |
| [**getMatchedTrack**](TracksApi.md#getmatchedtrack) | **GET** /tracks/{id} |  |



## createMatchedTrack

> MatchedTrackIdentifier createMatchedTrack(track, calculationMode)



Creates a complete track by triggering a matching calculation for it.

### Example

```ts
import {
  Configuration,
  TracksApi,
} from '';
import type { CreateMatchedTrackRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TracksApi(config);

  const body = {
    // Track
    track: ...,
    // CalculationMode | The calculationMode affects the quality and performance of the matching. (optional)
    calculationMode: ...,
  } satisfies CreateMatchedTrackRequest;

  try {
    const data = await api.createMatchedTrack(body);
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
| **track** | [Track](Track.md) |  | |
| **calculationMode** | `CalculationMode` | The calculationMode affects the quality and performance of the matching. | [Optional] [Defaults to `undefined`] [Enum: PERFORMANCE, STANDARD, QUALITY] |

### Return type

[**MatchedTrackIdentifier**](MatchedTrackIdentifier.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **202** | Response on success. |  -  |
| **0** | Response on failure. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteMatchedTrack

> deleteMatchedTrack(id)



Deletes a matched track specified by its ID.

### Example

```ts
import {
  Configuration,
  TracksApi,
} from '';
import type { DeleteMatchedTrackRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TracksApi(config);

  const body = {
    // string | The ID of the MatchedTrack.
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteMatchedTrackRequest;

  try {
    const data = await api.deleteMatchedTrack(body);
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
| **id** | `string` | The ID of the MatchedTrack. | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Response on success. |  -  |
| **0** | Response on failure. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getMatchedTrack

> MatchingResponse getMatchedTrack(id, results, maximumPollingPeriod)



Gets the results of a matching calculation specified by its ID.

### Example

```ts
import {
  Configuration,
  TracksApi,
} from '';
import type { GetMatchedTrackRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TracksApi(config);

  const body = {
    // string | The ID of the MatchedTrack.
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // Array<MatchedTrackResultType> | Selects which properties the MatchedTrack will contain. (optional)
    results: ...,
    // number | If the calculation is still running, this operation will be blocked and will not return before this period [ms] expires. If the calculation is completed, it will return immediately.    The default of 0 ms will cause the operation to return immediately in any case. Use a value > 0 to implement long polling to reduce the number of requests. See the [tutorial](https://developer.myptv.com/en/resources/tutorials/general/how-use-asynchronous-requests-ptv-developer-apis) on asynchronous requests for details. (optional)
    maximumPollingPeriod: 56,
  } satisfies GetMatchedTrackRequest;

  try {
    const data = await api.getMatchedTrack(body);
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
| **id** | `string` | The ID of the MatchedTrack. | [Defaults to `undefined`] |
| **results** | `Array<MatchedTrackResultType>` | Selects which properties the MatchedTrack will contain. | [Optional] |
| **maximumPollingPeriod** | `number` | If the calculation is still running, this operation will be blocked and will not return before this period [ms] expires. If the calculation is completed, it will return immediately.    The default of 0 ms will cause the operation to return immediately in any case. Use a value &gt; 0 to implement long polling to reduce the number of requests. See the [tutorial](https://developer.myptv.com/en/resources/tutorials/general/how-use-asynchronous-requests-ptv-developer-apis) on asynchronous requests for details. | [Optional] [Defaults to `0`] |

### Return type

[**MatchingResponse**](MatchingResponse.md)

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

