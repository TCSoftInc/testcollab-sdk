
# ScimTokenStatus

Non-secret status of a company\'s SCIM provisioning token (TCV-6663). Never contains the token itself.

## Properties

Name | Type
------------ | -------------
`enabled` | boolean
`configured` | boolean
`createdAt` | string
`lastRotatedAt` | string

## Example

```typescript
import type { ScimTokenStatus } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "enabled": true,
  "configured": true,
  "createdAt": 2026-07-03T10:00:00.000Z,
  "lastRotatedAt": 2026-07-03T10:00:00.000Z,
} satisfies ScimTokenStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ScimTokenStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


