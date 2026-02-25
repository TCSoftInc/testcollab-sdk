
# ReleaseReadinessSummary

Aggregated execution results across all test plans in the release, using the latest run (regression) of each test plan. 

## Properties

Name | Type
------------ | -------------
`total` | number
`passed` | number
`failed` | number
`blocked` | number
`skipped` | number
`unexecuted` | number
`passRate` | number

## Example

```typescript
import type { ReleaseReadinessSummary } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "total": 412,
  "passed": 360,
  "failed": 32,
  "blocked": 8,
  "skipped": 4,
  "unexecuted": 8,
  "passRate": 89.1,
} satisfies ReleaseReadinessSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


