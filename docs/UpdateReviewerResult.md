
# UpdateReviewerResult


## Properties

Name | Type
------------ | -------------
`id` | number
`status` | boolean
`message` | string
`reviewer` | string

## Example

```typescript
import type { UpdateReviewerResult } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "status": true,
  "message": Reviewer updated successfully,
  "reviewer": null,
} satisfies UpdateReviewerResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateReviewerResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


