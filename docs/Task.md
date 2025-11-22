
# Task


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | [ProjectMini](ProjectMini.md)
`user` | [UserMinified](UserMinified.md)
`title` | string
`completed` | boolean
`priority` | number
`startDate` | string
`endDate` | string
`href` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { Task } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": null,
  "user": null,
  "title": Chrome Test,
  "completed": false,
  "priority": 1,
  "startDate": 2019-04-26T00:00:00.000Z,
  "endDate": 2019-04-30T00:00:00.000Z,
  "href": /test_plans/1,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies Task

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Task
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


