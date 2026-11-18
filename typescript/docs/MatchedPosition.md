
# MatchedPosition

Represents the successful match of a position on the map including the matched segment and the deviation to the input position. For unsuccessful matches an empty object is returned.

## Properties

Name | Type
------------ | -------------
`latitude` | number
`longitude` | number
`segmentGeometry` | string
`matchDistance` | number
`angleDifference` | number
`segmentLocationDescriptors` | [SegmentLocationDescriptors](SegmentLocationDescriptors.md)
`segmentAttributes` | [SegmentAttributes](SegmentAttributes.md)
`lowEmissionZones` | [Array&lt;LowEmissionZoneDescriptors&gt;](LowEmissionZoneDescriptors.md)
`toll` | [Toll](Toll.md)
`warnings` | [Array&lt;Warning&gt;](Warning.md)

## Example

```typescript
import type { MatchedPosition } from ''

// TODO: Update the object below with actual values
const example = {
  "latitude": null,
  "longitude": null,
  "segmentGeometry": null,
  "matchDistance": null,
  "angleDifference": null,
  "segmentLocationDescriptors": null,
  "segmentAttributes": null,
  "lowEmissionZones": null,
  "toll": null,
  "warnings": null,
} satisfies MatchedPosition

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MatchedPosition
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


