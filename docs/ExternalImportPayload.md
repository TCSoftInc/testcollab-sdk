
# ExternalImportPayload


## Properties

Name | Type
------------ | -------------
`importType` | string
`project` | number
`sourceProject` | string
`credentials` | [ExternalImportCredentials](ExternalImportCredentials.md)
`credentialSecretRefs` | [ExternalImportCredentialSecretRefs](ExternalImportCredentialSecretRefs.md)
`options` | [ExternalImportOptions](ExternalImportOptions.md)

## Example

```typescript
import type { ExternalImportPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "importType": xray,
  "project": 42,
  "sourceProject": ABC,
  "credentials": null,
  "credentialSecretRefs": null,
  "options": null,
} satisfies ExternalImportPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


