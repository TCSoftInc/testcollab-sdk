
# DeleteAccountPayload

Payload for deleting a company account

## Properties

Name | Type
------------ | -------------
`company` | number
`confirmName` | string
`reason` | string

## Example

```typescript
import type { DeleteAccountPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "company": 1,
  "confirmName": My Company,
  "reason": No longer needed,
} satisfies DeleteAccountPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DeleteAccountPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


