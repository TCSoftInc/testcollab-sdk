
# ExternalImportTestConnectionPayload


## Properties

Name | Type
------------ | -------------
`importType` | string
`project` | number
`credentials` | [ExternalImportCredentials](ExternalImportCredentials.md)
`credentialSecretRefs` | [ExternalImportCredentialSecretRefs](ExternalImportCredentialSecretRefs.md)

## Example

```typescript
import type { ExternalImportTestConnectionPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "importType": xray,
  "project": 42,
  "credentials": null,
  "credentialSecretRefs": null,
} satisfies ExternalImportTestConnectionPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportTestConnectionPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


