
# SegmentLocationDescriptors

Describes the location of a segment. Not all descriptors are available for all segments.

## Properties

Name | Type
------------ | -------------
`countryName` | string
`countryCode` | string
`city` | string
`postalCode` | string
`street` | string

## Example

```typescript
import type { SegmentLocationDescriptors } from ''

// TODO: Update the object below with actual values
const example = {
  "countryName": null,
  "countryCode": null,
  "city": null,
  "postalCode": null,
  "street": null,
} satisfies SegmentLocationDescriptors

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SegmentLocationDescriptors
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


