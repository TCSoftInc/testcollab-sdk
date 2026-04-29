
# ExternalImportCredentialSecretRefs

Optional map of credential field keys to project secret names. The external import service resolves these references server-side using the destination TestCollab project\'s saved secrets when the selected adapter supports it. For xray imports, direct credential input is expected. 

## Properties

Name | Type
------------ | -------------
`xrayClientId` | string
`xrayClientSecret` | string
`jiraToken` | string

## Example

```typescript
import type { ExternalImportCredentialSecretRefs } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "xrayClientId": XRAY_CLIENT_ID,
  "xrayClientSecret": XRAY_CLIENT_SECRET,
  "jiraToken": JIRA_API_TOKEN,
} satisfies ExternalImportCredentialSecretRefs

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportCredentialSecretRefs
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


