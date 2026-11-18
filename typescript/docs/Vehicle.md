
# Vehicle

Describes a vehicle category with more specific vehicle characteristics.

## Properties

Name | Type
------------ | -------------
`vehicleCategory` | string
`timeRestrictions` | Array&lt;string&gt;
`fuelTypes` | Array&lt;string&gt;
`emissionStandards` | [Array&lt;EmissionStandard&gt;](EmissionStandard.md)
`vehicleAttributes` | { [key: string]: any; }

## Example

```typescript
import type { Vehicle } from ''

// TODO: Update the object below with actual values
const example = {
  "vehicleCategory": TRUCK,
  "timeRestrictions": null,
  "fuelTypes": null,
  "emissionStandards": null,
  "vehicleAttributes": {"max_total_weight":"3500"},
} satisfies Vehicle

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Vehicle
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


