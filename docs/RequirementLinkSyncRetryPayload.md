
# RequirementLinkSyncRetryPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`testcase` | number
`requirement` | number

## Example

```typescript
import type { RequirementLinkSyncRetryPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 42,
  "project": 28,
  "testcase": 1826,
  "requirement": 127,
} satisfies RequirementLinkSyncRetryPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RequirementLinkSyncRetryPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


