
# LowEmissionZoneDescriptors

Describes the low emission zone properties of a segment.

## Properties

Name | Type
------------ | -------------
`name` | string
`approvals` | Array&lt;string&gt;
`vehicleCategories` | Array&lt;string&gt;
`fuelTypes` | Array&lt;string&gt;
`vehicles` | [Array&lt;Vehicle&gt;](Vehicle.md)

## Example

```typescript
import type { LowEmissionZoneDescriptors } from ''

// TODO: Update the object below with actual values
const example = {
  "name": Firenze Ecozona,
  "approvals": null,
  "vehicleCategories": null,
  "fuelTypes": null,
  "vehicles": null,
} satisfies LowEmissionZoneDescriptors

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LowEmissionZoneDescriptors
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


