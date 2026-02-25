
# ReleaseReadiness

Aggregated readiness data for a release. Combines execution results, defect counts, coverage analysis, evidence metrics, and a computed Go/No-Go verdict across all test plans in the release. 

## Properties

Name | Type
------------ | -------------
`release` | [ReleaseMinified](.md)
`summary` | [ReleaseReadinessSummary](.md)
`defects` | [ReleaseReadinessDefects](.md)
`coverage` | [Array&lt;ReleaseReadinessCoverageItem&gt;](ReleaseReadinessCoverageItem.md)
`evidence` | [ReleaseReadinessEvidence](.md)
`comparison` | [ReleaseReadinessComparison](.md)
`verdict` | [ReleaseReadinessVerdict](.md)
`testPlans` | [Array&lt;ReleaseReadinessTestPlan&gt;](ReleaseReadinessTestPlan.md)
`requirementCoverage` | [ReleaseReadinessRequirementCoverage](.md)
`customFieldCoverage` | [Array&lt;ReleaseReadinessCustomFieldCoverage&gt;](ReleaseReadinessCustomFieldCoverage.md)
`configurationCoverage` | [Array&lt;ReleaseReadinessConfigurationCoverage&gt;](ReleaseReadinessConfigurationCoverage.md)

## Example

```typescript
import type { ReleaseReadiness } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "release": null,
  "summary": null,
  "defects": null,
  "coverage": null,
  "evidence": null,
  "comparison": null,
  "verdict": null,
  "testPlans": null,
  "requirementCoverage": null,
  "customFieldCoverage": null,
  "configurationCoverage": null,
} satisfies ReleaseReadiness

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadiness
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


