
# QacConversationMessage


## Properties

Name | Type
------------ | -------------
`id` | number
`thread` | number
`authorType` | string
`author` | [UserMinified](UserMinified.md)
`role` | string
`content` | string
`contentHtml` | string
`attachments` | [Array&lt;Upload&gt;](Upload.md)
`status` | string
`errorReason` | string
`tokenUsage` | [QacConversationTokenUsage](QacConversationTokenUsage.md)
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { QacConversationMessage } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 120,
  "thread": 45,
  "authorType": user,
  "author": null,
  "role": assistant,
  "content": Here are the steps to reproduce the issue.,
  "contentHtml": <p>Here are the steps to reproduce the issue.</p>,
  "attachments": null,
  "status": completed,
  "errorReason": LLM request failed,
  "tokenUsage": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies QacConversationMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QacConversationMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


