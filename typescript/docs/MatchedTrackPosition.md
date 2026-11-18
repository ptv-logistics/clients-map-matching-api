
# MatchedTrackPosition

Detailed information about a position on a track matched on a map.

## Properties

Name | Type
------------ | -------------
`matchType` | [MatchType](MatchType.md)
`timestamp` | Date
`distanceFromPreviousMatch` | number
`latitude` | number
`longitude` | number
`segmentGeometry` | string
`matchDistance` | number
`angleDifference` | number
`segmentAttributes` | [SegmentAttributes](SegmentAttributes.md)

## Example

```typescript
import type { MatchedTrackPosition } from ''

// TODO: Update the object below with actual values
const example = {
  "matchType": null,
  "timestamp": 2024-10-24T06:00Z,
  "distanceFromPreviousMatch": null,
  "latitude": null,
  "longitude": null,
  "segmentGeometry": null,
  "matchDistance": null,
  "angleDifference": null,
  "segmentAttributes": null,
} satisfies MatchedTrackPosition

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MatchedTrackPosition
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


