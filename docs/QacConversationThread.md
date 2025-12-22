
# QacConversationThread


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`company` | number
`createdBy` | [UserMinified](UserMinified.md)
`title` | string
`status` | string
`sourceUrl` | string
`contextRefs` | { [key: string]: any; }
`messagesCount` | number
`lastMessageAt` | string
`lastMessagePreview` | string
`pinned` | boolean
`metadata` | { [key: string]: any; }
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { QacConversationThread } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 45,
  "project": 12,
  "company": 3,
  "createdBy": null,
  "title": Checkout regression draft,
  "status": open,
  "sourceUrl": https://app.testcollab.io/project/12/test_cases/101,
  "contextRefs": null,
  "messagesCount": 14,
  "lastMessageAt": 2019-04-30T17:11:24.000Z,
  "lastMessagePreview": Drafted 5 test cases for checkout happy path.,
  "pinned": false,
  "metadata": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies QacConversationThread

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QacConversationThread
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


