
# RiskAssociation


## Properties

Name | Type
------------ | -------------
`targetType` | string
`targetId` | number
`targetDisplayNumber` | number
`targetTitle` | string
`relationType` | string
`createdAt` | string

## Example

```typescript
import type { RiskAssociation } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "targetType": test_case,
  "targetId": 204,
  "targetDisplayNumber": 204,
  "targetTitle": Verify payment authorization under concurrent sessions,
  "relationType": verifies,
  "createdAt": 2026-04-30T17:11:24.000Z,
} satisfies RiskAssociation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RiskAssociation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


