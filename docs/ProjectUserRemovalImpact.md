
# ProjectUserRemovalImpact

Actionable assignments that belong to a project member, calculated before the member is removed from the project. Completed executions and historical records are not counted - they are never rewritten.

## Properties

Name | Type
------------ | -------------
`total` | number
`defaultAssignments` | number
`planCaseAssignments` | number
`configurationAssignments` | number
`affectedTestCases` | number
`affectedTestPlans` | number

## Example

```typescript
import type { ProjectUserRemovalImpact } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "total": 12,
  "defaultAssignments": 3,
  "planCaseAssignments": 6,
  "configurationAssignments": 2,
  "affectedTestCases": 8,
  "affectedTestPlans": 2,
} satisfies ProjectUserRemovalImpact

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectUserRemovalImpact
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


