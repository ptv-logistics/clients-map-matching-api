
# MatchedTrack

Contains the result of the matched track.

## Properties

Name | Type
------------ | -------------
`id` | string
`distance` | number
`paths` | [Array&lt;MatchedPath&gt;](MatchedPath.md)
`geometry` | string
`trackPositions` | [Array&lt;MatchedTrackPosition&gt;](MatchedTrackPosition.md)

## Example

```typescript
import type { MatchedTrack } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "distance": null,
  "paths": null,
  "geometry": null,
  "trackPositions": null,
} satisfies MatchedTrack

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MatchedTrack
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


