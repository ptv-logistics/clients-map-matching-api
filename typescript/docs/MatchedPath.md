
# MatchedPath

Detailed information about a continuous part of a matched track.

## Properties

Name | Type
------------ | -------------
`distance` | number
`startTime` | Date
`startTrackPositionIndex` | number
`endTime` | Date
`endTrackPositionIndex` | number
`routeId` | string

## Example

```typescript
import type { MatchedPath } from ''

// TODO: Update the object below with actual values
const example = {
  "distance": null,
  "startTime": 2024-10-24T06:00Z,
  "startTrackPositionIndex": null,
  "endTime": 2024-10-24T06:30Z,
  "endTrackPositionIndex": null,
  "routeId": null,
} satisfies MatchedPath

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MatchedPath
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


