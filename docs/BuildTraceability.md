
# BuildTraceability

Aggregated traceability for a build (TCV-6726). Provider-neutral: the same shape is returned whether the project is connected to Azure DevOps or managed manually; the client decides which sections to surface. 

## Properties

Name | Type
------------ | -------------
`results` | [BuildTraceabilityResults](BuildTraceabilityResults.md)
`testPlans` | [Array&lt;BuildTestPlanResult&gt;](BuildTestPlanResult.md)
`riskCoverage` | [BuildRiskCoverage](BuildRiskCoverage.md)
`defects` | [Array&lt;BuildDefect&gt;](BuildDefect.md)
`defectSummary` | [BuildTraceabilityDefectSummary](BuildTraceabilityDefectSummary.md)
`workItems` | [Array&lt;BuildWorkItem&gt;](BuildWorkItem.md)

## Example

```typescript
import type { BuildTraceability } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "results": null,
  "testPlans": null,
  "riskCoverage": null,
  "defects": null,
  "defectSummary": null,
  "workItems": null,
} satisfies BuildTraceability

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BuildTraceability
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


