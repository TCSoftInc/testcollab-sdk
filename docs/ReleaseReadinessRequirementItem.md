
# ReleaseReadinessRequirementItem

Coverage data for a single requirement associated with the release. 

## Properties

Name | Type
------------ | -------------
`requirementId` | number
`requirementKey` | string
`title` | string
`totalLinkedCases` | number
`casesInRelease` | number
`executed` | number
`passed` | number
`failed` | number
`coverageStatus` | string

## Example

```typescript
import type { ReleaseReadinessRequirementItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "requirementId": 101,
  "requirementKey": REQ-42,
  "title": User can reset password via email,
  "totalLinkedCases": 8,
  "casesInRelease": 5,
  "executed": 4,
  "passed": 3,
  "failed": 1,
  "coverageStatus": partially_covered,
} satisfies ReleaseReadinessRequirementItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessRequirementItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


