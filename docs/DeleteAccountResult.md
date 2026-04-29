
# DeleteAccountResult


## Properties

Name | Type
------------ | -------------
`status` | boolean
`queue` | [DeleteAccountResultQueue](DeleteAccountResultQueue.md)
`message` | string

## Example

```typescript
import type { DeleteAccountResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": true,
  "queue": null,
  "message": Account deletion has been queued,
} satisfies DeleteAccountResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeleteAccountResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


