
# QueuePayload


## Properties

Name | Type
------------ | -------------
`id` | number
`task` | string
`parameters` | string
`company` | number
`queueName` | string

## Example

```typescript
import type { QueuePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "task": bulkDelete,
  "parameters": {},
  "company": 1,
  "queueName": null,
} satisfies QueuePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QueuePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


