
# ScimTokenGenerated

Result of generating/rotating a SCIM provisioning token (TCV-6663). The plaintext token is returned exactly once and only its hash is stored server-side.

## Properties

Name | Type
------------ | -------------
`token` | string
`createdAt` | string
`lastRotatedAt` | string

## Example

```typescript
import type { ScimTokenGenerated } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "token": b5f1c0e3a9d84f7c8e2b1a6d4c3f9e0a1b2c3d4e5f60718293a4b5c6d7e8f9012,
  "createdAt": 2026-07-03T10:00:00.000Z,
  "lastRotatedAt": 2026-07-03T10:00:00.000Z,
} satisfies ScimTokenGenerated

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ScimTokenGenerated
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


