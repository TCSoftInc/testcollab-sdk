
# ExternalImportCredentialField


## Properties

Name | Type
------------ | -------------
`key` | string
`label` | string
`type` | string
`placeholder` | string
`supportsProjectSecret` | boolean

## Example

```typescript
import type { ExternalImportCredentialField } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "key": xray_client_id,
  "label": Xray Client ID,
  "type": text,
  "placeholder": mycompany.atlassian.net,
  "supportsProjectSecret": true,
} satisfies ExternalImportCredentialField

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportCredentialField
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


