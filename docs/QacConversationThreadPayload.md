
# QacConversationThreadPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`company` | number
`title` | string
`status` | string
`sourceUrl` | string
`contextRefs` | { [key: string]: any; }
`metadata` | { [key: string]: any; }

## Example

```typescript
import type { QacConversationThreadPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 12,
  "company": 3,
  "title": Checkout regression draft,
  "status": open,
  "sourceUrl": https://app.testcollab.io/project/12/test_cases/101,
  "contextRefs": null,
  "metadata": null,
} satisfies QacConversationThreadPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QacConversationThreadPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


