
# TestCaseCommentPayload


## Properties

Name | Type
------------ | -------------
`comment` | string
`testCase` | number
`project` | number
`attachments` | Array&lt;string&gt;
`mentions` | Array&lt;string&gt;
`parentId` | number

## Example

```typescript
import type { TestCaseCommentPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "comment": sample text,
  "testCase": 1,
  "project": 1,
  "attachments": null,
  "mentions": null,
  "parentId": 0,
} satisfies TestCaseCommentPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseCommentPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


