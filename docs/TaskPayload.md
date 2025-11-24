
# TaskPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`company` | number
`title` | string
`completed` | boolean
`href` | string
`priority` | number
`startDate` | string
`endDate` | string

## Example

```typescript
import type { TaskPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "company": 1,
  "title": Chrome Test,
  "completed": true,
  "href": /test_plans/1,
  "priority": 1,
  "startDate": 2019-04-26T00:00:00.000Z,
  "endDate": 2019-04-30T00:00:00.000Z,
} satisfies TaskPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TaskPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


