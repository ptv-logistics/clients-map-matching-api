
# TrackPosition

Describes a position which belongs to a track with additional track related attributes.

## Properties

Name | Type
------------ | -------------
`latitude` | number
`longitude` | number
`heading` | number
`distanceFromPreviousPosition` | number
`timestamp` | Date

## Example

```typescript
import type { TrackPosition } from ''

// TODO: Update the object below with actual values
const example = {
  "latitude": 49.480301,
  "longitude": 6.110667,
  "heading": 45,
  "distanceFromPreviousPosition": null,
  "timestamp": 2024-10-24T06:00Z,
} satisfies TrackPosition

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrackPosition
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


