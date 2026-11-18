
# CalculationMode

Enumeration to define the calculation behavior of the matching, i.e. if the focus of calculation is on performance, quality or both.    * `PERFORMANCE` - The matching focuses on performance. This means to take into account a higher number of failed matches and in the case of track matching that the matched track may be split into several paths.    * `STANDARD` - The matching chooses a standard trade-off between quality and performance.    * `QUALITY` - The matching focuses on high solution quality. This means that as many as possible of the input positions are matched and taken into account. Though the processing time of the request can be high.

## Properties

Name | Type
------------ | -------------

## Example

```typescript
import type { CalculationMode } from ''

// TODO: Update the object below with actual values
const example = {
} satisfies CalculationMode

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CalculationMode
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


