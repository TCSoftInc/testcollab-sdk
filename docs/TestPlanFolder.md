
# TestPlanFolder


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`title` | string
`parentId` | number
`sortOrder` | number
`testplancount` | number
`createdBy` | number
`description` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { TestPlanFolder } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "title": My folder,
  "parentId": 1,
  "sortOrder": 1,
  "testplancount": 1,
  "createdBy": 1,
  "description": My folder description,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies TestPlanFolder

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanFolder
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


