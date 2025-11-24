
# Suite


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`description` | string
`parentId` | number
`order` | number
`createdBy` | number
`isReference` | boolean
`sourceId` | number
`sourceProject` | number
`isMainLink` | boolean

## Example

```typescript
import type { Suite } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "title": Suite 1,
  "description": Used for abc, def...,
  "parentId": null,
  "order": 1,
  "createdBy": 1,
  "isReference": false,
  "sourceId": 1,
  "sourceProject": 1,
  "isMainLink": false,
} satisfies Suite

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Suite
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


