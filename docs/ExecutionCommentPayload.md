
# ExecutionCommentPayload


## Properties

Name | Type
------------ | -------------
`comment` | string
`executedTestCase` | number
`project` | number
`mentions` | Array&lt;string&gt;

## Example

```typescript
import type { ExecutionCommentPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "comment": sample text,
  "executedTestCase": 1,
  "project": 1,
  "mentions": null,
} satisfies ExecutionCommentPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExecutionCommentPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


