
# QacConversationMessagePayload


## Properties

Name | Type
------------ | -------------
`thread` | number
`authorType` | string
`role` | string
`content` | string
`contentHtml` | string
`attachments` | Array&lt;number&gt;
`metadata` | { [key: string]: any; }

## Example

```typescript
import type { QacConversationMessagePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "thread": 45,
  "authorType": user,
  "role": assistant,
  "content": Draft a regression test outline for checkout.,
  "contentHtml": <p>Draft a regression test outline for checkout.</p>,
  "attachments": null,
  "metadata": null,
} satisfies QacConversationMessagePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QacConversationMessagePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


