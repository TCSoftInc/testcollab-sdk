
# ReleaseReadinessRunHistory

Execution results across every run of every test plan in the release, not only the latest run. Each execution of each run counts once, so a case that failed in two runs counts twice. `summary` on the readiness answer says where the release stands now; this says how often its cases passed, failed or were skipped on the way there. 

## Properties

Name | Type
------------ | -------------
`runs` | number
`summary` | [ReleaseReadinessSummary](.md)

## Example

```typescript
import type { ReleaseReadinessRunHistory } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "runs": 13,
  "summary": null,
} satisfies ReleaseReadinessRunHistory

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessRunHistory
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


