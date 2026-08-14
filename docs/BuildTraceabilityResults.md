
# BuildTraceabilityResults

Execution results summed across every test plan linked to this build.

## Properties

Name | Type
------------ | -------------
`total` | number
`passed` | number
`failed` | number
`blocked` | number
`skipped` | number
`unexecuted` | number
`executed` | number
`byStatus` | { [key: string]: number; }
`bySource` | { [key: string]: number; }

## Example

```typescript
import type { BuildTraceabilityResults } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "total": 148,
  "passed": 141,
  "failed": 4,
  "blocked": 2,
  "skipped": 1,
  "unexecuted": 0,
  "executed": 148,
  "byStatus": null,
  "bySource": null,
} satisfies BuildTraceabilityResults

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BuildTraceabilityResults
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


