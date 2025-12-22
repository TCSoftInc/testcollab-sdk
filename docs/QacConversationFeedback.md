
# QacConversationFeedback


## Properties

Name | Type
------------ | -------------
`id` | number
`message` | number
`givenBy` | [UserMinified](UserMinified.md)
`rating` | string
`reason` | string
`comment` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { QacConversationFeedback } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 5,
  "message": 120,
  "givenBy": null,
  "rating": up,
  "reason": irrelevant,
  "comment": The suggestion missed mobile edge cases.,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies QacConversationFeedback

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QacConversationFeedback
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


