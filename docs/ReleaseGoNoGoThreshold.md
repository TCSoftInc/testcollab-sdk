
# ReleaseGoNoGoThreshold

Configurable thresholds that determine the auto-computed Go/No-Go verdict for a release. All fields are optional — only configured thresholds are evaluated. 

## Properties

Name | Type
------------ | -------------
`minPassRate` | number
`maxOpenDefects` | number
`minEvidenceCoverage` | number

## Example

```typescript
import type { ReleaseGoNoGoThreshold } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "minPassRate": 95,
  "maxOpenDefects": 0,
  "minEvidenceCoverage": 80,
} satisfies ReleaseGoNoGoThreshold

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseGoNoGoThreshold
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


