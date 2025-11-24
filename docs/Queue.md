
# Queue


## Properties

Name | Type
------------ | -------------
`id` | number
`task` | string
`parameters` | string
`status` | number
`percentDone` | number
`createdAt` | string
`updatedAt` | string
`results` | string

## Example

```typescript
import type { Queue } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "task": bulkDelete,
  "parameters": {},
  "status": 1,
  "percentDone": 10,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
  "results": {},
} satisfies Queue

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Queue
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


