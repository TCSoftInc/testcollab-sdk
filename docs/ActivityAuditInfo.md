
# ActivityAuditInfo

Additional metadata for the activity (e.g. release name, old/new verdict)

## Properties

Name | Type
------------ | -------------
`releaseName` | string
`oldVerdict` | string
`newVerdict` | string

## Example

```typescript
import type { ActivityAuditInfo } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "releaseName": v1,
  "oldVerdict": No-Go,
  "newVerdict": Go,
} satisfies ActivityAuditInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ActivityAuditInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


