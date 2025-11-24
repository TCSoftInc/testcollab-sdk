
# Activity


## Properties

Name | Type
------------ | -------------
`entity` | string
`entityId` | number
`entityTitle` | string
`testCaseTitle` | string
`testPlanTitle` | string
`project` | [ProjectMini](ProjectMini.md)
`activityType` | string
`user` | [User](User.md)
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { Activity } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "entity": TestCase,
  "entityId": 1,
  "entityTitle": test 1,
  "testCaseTitle": test 1,
  "testPlanTitle": test plan 1,
  "project": null,
  "activityType": add,
  "user": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies Activity

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Activity
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


