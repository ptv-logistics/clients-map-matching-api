
# MatchedTrackResultType

Select properties for the MatchedTrack.    * `PATHS` - The MatchedTrack will contain the paths.    * `GEOMETRY` - The MatchedTrack will contain the geometry.    * `TRACK_POSITIONS` - The MatchedTrack will contain the track positions.    * `ROUTE_ID` - The MatchedTrack will contain the route ID for each path. PATHS will automatically be included.    * `SEGMENT_ATTRIBUTES` - The MatchedTrack will contain segment attributes for the track positions.  TRACK_POSITIONS will automatically be included.

## Properties

Name | Type
------------ | -------------

## Example

```typescript
import type { MatchedTrackResultType } from ''

// TODO: Update the object below with actual values
const example = {
} satisfies MatchedTrackResultType

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MatchedTrackResultType
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


