
# DeleteAccountResultQueue

Queue record for tracking deletion progress

## Properties

Name | Type
------------ | -------------
`id` | number
`status` | number
`percentDone` | number

## Example

```typescript
import type { DeleteAccountResultQueue } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "status": 0,
  "percentDone": 0,
} satisfies DeleteAccountResultQueue

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeleteAccountResultQueue
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


