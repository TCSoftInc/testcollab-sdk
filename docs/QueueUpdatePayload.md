
# QueueUpdatePayload


## Properties

Name | Type
------------ | -------------
`status` | number
`percentDone` | number
`company` | number
`results` | string

## Example

```typescript
import type { QueueUpdatePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "status": 2,
  "percentDone": 20,
  "company": 1,
  "results": {},
} satisfies QueueUpdatePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QueueUpdatePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


