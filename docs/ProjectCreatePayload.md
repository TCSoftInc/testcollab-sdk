
# ProjectCreatePayload


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`description` | string
`importUsers` | number
`issueManagerProfile` | number
`importIssueManagerSettings` | number
`company` | number

## Example

```typescript
import type { ProjectCreatePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Crowd Vox,
  "description": QA workspace for the customer web app,
  "importUsers": 2,
  "issueManagerProfile": null,
  "importIssueManagerSettings": 2,
  "company": 1,
} satisfies ProjectCreatePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectCreatePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


