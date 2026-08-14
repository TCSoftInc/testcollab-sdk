
# BuildTraceabilityDefectSummary

Roll-up of the defects raised against the build\'s plans.

## Properties

Name | Type
------------ | -------------
`total` | number
`open` | number
`closed` | number

## Example

```typescript
import type { BuildTraceabilityDefectSummary } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "total": 5,
  "open": 2,
  "closed": 3,
} satisfies BuildTraceabilityDefectSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BuildTraceabilityDefectSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


