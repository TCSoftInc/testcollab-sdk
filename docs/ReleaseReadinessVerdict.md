
# ReleaseReadinessVerdict

Computed Go/No-Go verdict based on the release\'s go_no_go_threshold settings compared against actual metrics. 

## Properties

Name | Type
------------ | -------------
`result` | string
`reasons` | Array&lt;string&gt;

## Example

```typescript
import type { ReleaseReadinessVerdict } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "result": no_go,
  "reasons": ["Pass rate 89.1% is below threshold of 95%","3 open blockers exceeds maximum of 0"],
} satisfies ReleaseReadinessVerdict

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessVerdict
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


