
# BulkLinkTestCasesPayload


## Properties

Name | Type
------------ | -------------
`ids` | Array&lt;number&gt;
`project` | number
`issueKey` | string
`issueId` | number
`imProjectId` | string
`imInstanceId` | string
`im` | string

## Example

```typescript
import type { BulkLinkTestCasesPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "ids": [1,2],
  "project": 3,
  "issueKey": PG-1,
  "issueId": 1,
  "imProjectId": null,
  "imInstanceId": null,
  "im": JIRA,
} satisfies BulkLinkTestCasesPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BulkLinkTestCasesPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


