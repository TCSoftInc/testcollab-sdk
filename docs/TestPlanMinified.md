
# TestPlanMinified


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`priority` | number
`status` | number
`testPlanFolder` | number
`startDate` | string
`endDate` | string
`createdAt` | string
`customFields` | [Array&lt;CustomFieldCollectionOutput&gt;](CustomFieldCollectionOutput.md)
`isPublic` | number

## Example

```typescript
import type { TestPlanMinified } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "title": My first test plan,
  "priority": 1,
  "status": 1,
  "testPlanFolder": 1,
  "startDate": 2019-04-30T17:11:24.000Z,
  "endDate": 2019-09-30T17:11:24.000Z,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "customFields": null,
  "isPublic": null,
} satisfies TestPlanMinified

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanMinified
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


