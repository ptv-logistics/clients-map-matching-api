
# MatchingResponse

Contains the results of a matching calculation. If the \'status\' is \'RUNNING\', the matching calculation is still running and no further properties are set. If the \'status\' is \'SUCCEEDED\', the matching result is present as property \'matchedTrack\'. If the \'status\' is \'FAILED\', the failure result is present as property \'error\'.

## Properties

Name | Type
------------ | -------------
`status` | [MatchingStatus](MatchingStatus.md)
`matchedTrack` | [MatchedTrack](MatchedTrack.md)
`error` | [ErrorResponse](ErrorResponse.md)
`warnings` | [Array&lt;Warning&gt;](Warning.md)

## Example

```typescript
import type { MatchingResponse } from ''

// TODO: Update the object below with actual values
const example = {
  "status": null,
  "matchedTrack": null,
  "error": null,
  "warnings": null,
} satisfies MatchingResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MatchingResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


