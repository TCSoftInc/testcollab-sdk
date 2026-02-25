
# Release


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`description` | string
`status` | string
`targetDate` | string
`releaseDate` | string
`goNoGoThreshold` | [ReleaseGoNoGoThreshold](.md)
`isPublic` | boolean
`publicToken` | string
`testPlans` | [Array&lt;TestPlanMinified&gt;](TestPlanMinified.md)
`requirements` | [Array&lt;RequirementMinified&gt;](RequirementMinified.md)
`project` | number
`createdBy` | [UserMinified](.md)
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { Release } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": v2.4.0,
  "description": Sprint 23 release with payment module updates,
  "status": in_progress,
  "targetDate": 2025-03-15,
  "releaseDate": 2025-03-14,
  "goNoGoThreshold": null,
  "isPublic": false,
  "publicToken": a1b2c3d4-e5f6-7890-abcd-ef1234567890,
  "testPlans": null,
  "requirements": null,
  "project": 1,
  "createdBy": null,
  "createdAt": 2025-02-11T10:00:00.000Z,
  "updatedAt": 2025-02-11T10:00:00.000Z,
} satisfies Release

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Release
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


