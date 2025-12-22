
# QacConversationTokenUsage


## Properties

Name | Type
------------ | -------------
`promptTokens` | number
`completionTokens` | number
`totalTokens` | number

## Example

```typescript
import type { QacConversationTokenUsage } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "promptTokens": 512,
  "completionTokens": 1024,
  "totalTokens": 1536,
} satisfies QacConversationTokenUsage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QacConversationTokenUsage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


