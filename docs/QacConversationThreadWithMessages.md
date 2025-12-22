
# QacConversationThreadWithMessages


## Properties

Name | Type
------------ | -------------
`thread` | [QacConversationThread](QacConversationThread.md)
`messages` | [Array&lt;QacConversationMessage&gt;](QacConversationMessage.md)

## Example

```typescript
import type { QacConversationThreadWithMessages } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "thread": null,
  "messages": null,
} satisfies QacConversationThreadWithMessages

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QacConversationThreadWithMessages
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


