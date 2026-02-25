
# ReleaseReadinessRequirementCoverage

Requirement coverage analysis for the release. Shows how well the requirements linked to this release are covered by test execution. 

## Properties

Name | Type
------------ | -------------
`summary` | [ReleaseReadinessRequirementSummary](.md)
`items` | [Array&lt;ReleaseReadinessRequirementItem&gt;](ReleaseReadinessRequirementItem.md)

## Example

```typescript
import type { ReleaseReadinessRequirementCoverage } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "summary": null,
  "items": null,
} satisfies ReleaseReadinessRequirementCoverage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessRequirementCoverage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


