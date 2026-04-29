
# ExternalImportAdapter


## Properties

Name | Type
------------ | -------------
`type` | string
`name` | string
`icon` | string
`credentialFields` | [Array&lt;ExternalImportCredentialField&gt;](ExternalImportCredentialField.md)
`optionsSchema` | [ExternalImportOptions](ExternalImportOptions.md)

## Example

```typescript
import type { ExternalImportAdapter } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "type": xray,
  "name": Jira + Xray,
  "icon": xray.svg,
  "credentialFields": null,
  "optionsSchema": null,
} satisfies ExternalImportAdapter

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportAdapter
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


