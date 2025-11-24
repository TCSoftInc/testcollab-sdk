
# SystemStatus


## Properties

Name | Type
------------ | -------------
`status` | string
`version` | string
`deployedOn` | string

## Example

```typescript
import type { SystemStatus } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": ready,
  "version": 2.0.19,
  "deployedOn": Mon Feb 22 18:00:53 IST 2021,
} satisfies SystemStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SystemStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


