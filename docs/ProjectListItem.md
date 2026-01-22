
# ProjectListItem


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`description` | string
`archived` | boolean
`team` | [Array&lt;ProjectUserMinified&gt;](ProjectUserMinified.md)
`activity` | string
`createdAt` | string
`updatedAt` | string
`isSample` | boolean
`testCaseCount` | number
`testPlanCount` | number

## Example

```typescript
import type { ProjectListItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Crowd Vox,
  "description": QA workspace for the customer web app,
  "archived": false,
  "team": null,
  "activity": 2017-06-05,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
  "isSample": false,
  "testCaseCount": 128,
  "testPlanCount": 7,
} satisfies ProjectListItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectListItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


