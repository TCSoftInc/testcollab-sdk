
# QueueStatus


## Properties

Name | Type
------------ | -------------
`status` | string
`percent` | number

## Example

```typescript
import type { QueueStatus } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": started,
  "percent": 20,
} satisfies QueueStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QueueStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


