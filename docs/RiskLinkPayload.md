
# RiskLinkPayload


## Properties

Name | Type
------------ | -------------
`targetType` | string
`targetId` | number
`relationType` | string

## Example

```typescript
import type { RiskLinkPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "targetType": test_case,
  "targetId": 204,
  "relationType": verifies,
} satisfies RiskLinkPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RiskLinkPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


