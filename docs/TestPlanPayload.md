
# TestPlanPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`archived` | boolean
`title` | string
`priority` | number
`status` | number
`testPlanFolder` | number
`description` | string
`startDate` | string
`endDate` | string
`project` | number
`customFields` | [Array&lt;CustomFieldInputPayload&gt;](CustomFieldInputPayload.md)

## Example

```typescript
import type { TestPlanPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "archived": false,
  "title": My first test plan,
  "priority": 1,
  "status": 1,
  "testPlanFolder": 1,
  "description": information about test plan,
  "startDate": 2020-10-31,
  "endDate": 2020-10-28,
  "project": 1,
  "customFields": null,
} satisfies TestPlanPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


