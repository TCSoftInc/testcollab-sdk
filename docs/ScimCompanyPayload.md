
# ScimCompanyPayload

Identifies the company whose SCIM provisioning token is being managed (TCV-6663).

## Properties

Name | Type
------------ | -------------
`company` | number

## Example

```typescript
import type { ScimCompanyPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "company": 5004,
} satisfies ScimCompanyPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ScimCompanyPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


