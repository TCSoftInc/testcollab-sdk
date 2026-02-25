
# ReleaseReadinessTestPlan

Per-test-plan readiness summary within a release, showing the latest run\'s results. 

## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`status` | number
`latestRun` | [ReleaseReadinessTestPlanRun](.md)
`results` | [ResultSummary](.md)

## Example

```typescript
import type { ReleaseReadinessTestPlan } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 5,
  "title": Regression - Payment Module,
  "status": 3,
  "latestRun": null,
  "results": null,
} satisfies ReleaseReadinessTestPlan

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessTestPlan
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


