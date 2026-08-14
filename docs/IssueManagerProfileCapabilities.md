
# IssueManagerProfileCapabilities

What an Azure DevOps connection is actually allowed to do, detected by probing the live Azure DevOps APIs. Each capability is `connected` (the connection can access it), `no_access` (the granted permissions do not cover it), or `unknown` (access could not be determined, e.g. the probe failed or the profile has no project selected yet). 

## Properties

Name | Type
------------ | -------------
`workItems` | string
`deployments` | string
`pipelines` | string
`serviceHooks` | string
`checkedAt` | string

## Example

```typescript
import type { IssueManagerProfileCapabilities } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "workItems": connected,
  "deployments": no_access,
  "pipelines": no_access,
  "serviceHooks": no_access,
  "checkedAt": 2026-07-22T10:30:00.000Z,
} satisfies IssueManagerProfileCapabilities

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as IssueManagerProfileCapabilities
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


