
# TrashItem


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`itemType` | string
`itemId` | number
`title` | string
`parentId` | number
`deletedBy` | number
`deletedByName` | string
`deletedAt` | string
`expiresAt` | string

## Example

```typescript
import type { TrashItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 42,
  "project": 8,
  "itemType": test_case,
  "itemId": 123,
  "title": Sign in with a valid password,
  "parentId": 17,
  "deletedBy": 5019,
  "deletedByName": Alex,
  "deletedAt": 2026-09-28T10:00:00.000Z,
  "expiresAt": 2026-11-27T10:00:00.000Z,
} satisfies TrashItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrashItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


