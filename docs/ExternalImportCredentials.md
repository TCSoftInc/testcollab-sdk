
# ExternalImportCredentials

Free-form credentials object whose keys are determined by the adapter\'s credential_fields schema. For the xray adapter the expected keys are xray_client_id, xray_client_secret, jira_host, jira_email and jira_token. Sensitive fields can be sent encrypted from the UI using the `tcenc:` prefix. The backend decrypts these values before validation/import. 

## Properties

Name | Type
------------ | -------------
`xrayClientId` | string
`xrayClientSecret` | string
`jiraHost` | string
`jiraEmail` | string
`jiraToken` | string

## Example

```typescript
import type { ExternalImportCredentials } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "xrayClientId": ABCDEF1234567890,
  "xrayClientSecret": secret-value,
  "jiraHost": mycompany.atlassian.net,
  "jiraEmail": user@mycompany.com,
  "jiraToken": jira-api-token,
} satisfies ExternalImportCredentials

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportCredentials
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


