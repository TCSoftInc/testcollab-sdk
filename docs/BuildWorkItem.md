
# BuildWorkItem


## Properties

Name | Type
------------ | -------------
`provider` | string
`profileId` | number
`issueKey` | string
`issueId` | number
`title` | string
`issueType` | string
`issueStatus` | string
`issueUrl` | string
`syncStatus` | string
`testcaseCount` | number
`testcases` | [Array&lt;BuildWorkItemTestcase&gt;](BuildWorkItemTestcase.md)

## Example

```typescript
import type { BuildWorkItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "provider": azuredevops,
  "profileId": null,
  "issueKey": 1842,
  "issueId": 1842,
  "title": Prevent duplicate settlement retries,
  "issueType": User Story,
  "issueStatus": Active,
  "issueUrl": https://dev.azure.com/example/Payments/_workitems/edit/1842,
  "syncStatus": null,
  "testcaseCount": 2,
  "testcases": null,
} satisfies BuildWorkItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BuildWorkItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


