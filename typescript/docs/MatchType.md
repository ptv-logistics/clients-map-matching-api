
# MatchType

Gives information on the result of this match, i.e. whether the position was matched successfully or whether the position is considered as part of the track or not.    * `MATCH_SUCCESSFUL` - The position was matched successfully.    * `MATCH_FAILED` - The position could not be matched.    * `NOT_CONSIDERED` - The position was not considered.

## Properties

Name | Type
------------ | -------------

## Example

```typescript
import type { MatchType } from ''

// TODO: Update the object below with actual values
const example = {
} satisfies MatchType

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MatchType
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


