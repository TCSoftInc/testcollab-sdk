
# TestCaseReviewPayload


## Properties

Name | Type
------------ | -------------
`actionType` | string
`project` | number
`comment` | string

## Example

```typescript
import type { TestCaseReviewPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "actionType": null,
  "project": 1,
  "comment": null,
} satisfies TestCaseReviewPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseReviewPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


