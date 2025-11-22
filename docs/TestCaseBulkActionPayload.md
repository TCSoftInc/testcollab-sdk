
# TestCaseBulkActionPayload


## Properties

Name | Type
------------ | -------------
`actionType` | string
`project` | number
`testcaseIds` | Array&lt;number&gt;
`resume` | boolean
`resumeFrom` | number
`editParams` | [TestCaseBulkActionEditPayload](TestCaseBulkActionEditPayload.md)
`reviewers` | Array&lt;number&gt;

## Example

```typescript
import type { TestCaseBulkActionPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "actionType": null,
  "project": 1,
  "testcaseIds": null,
  "resume": null,
  "resumeFrom": null,
  "editParams": null,
  "reviewers": null,
} satisfies TestCaseBulkActionPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseBulkActionPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


