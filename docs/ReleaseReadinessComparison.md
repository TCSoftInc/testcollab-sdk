
# ReleaseReadinessComparison

Comparison of this release\'s readiness metrics against the previous release in the same project. Null if no previous release exists. 

## Properties

Name | Type
------------ | -------------
`previousRelease` | [ReleaseMinified](.md)
`previousPassRate` | number
`passRateDelta` | number
`previousOpenDefects` | number

## Example

```typescript
import type { ReleaseReadinessComparison } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "previousRelease": null,
  "previousPassRate": 94.1,
  "passRateDelta": -5,
  "previousOpenDefects": 5,
} satisfies ReleaseReadinessComparison

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessComparison
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


