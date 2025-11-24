
# TestCaseRevisionReviewData


## Properties

Name | Type
------------ | -------------
`title` | string
`suite` | number
`description` | string
`steps` | [Array&lt;Step&gt;](Step.md)
`stepsParsed` | [Array&lt;StepParsed&gt;](StepParsed.md)
`priority` | number
`customFields` | [Array&lt;CustomFieldCollectionOutput&gt;](CustomFieldCollectionOutput.md)
`tags` | [Array&lt;Tag&gt;](Tag.md)
`requirements` | [Array&lt;Requirement&gt;](Requirement.md)
`attachments` | [Array&lt;Upload&gt;](Upload.md)

## Example

```typescript
import type { TestCaseRevisionReviewData } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "title": null,
  "suite": null,
  "description": null,
  "steps": null,
  "stepsParsed": null,
  "priority": null,
  "customFields": null,
  "tags": null,
  "requirements": null,
  "attachments": null,
} satisfies TestCaseRevisionReviewData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseRevisionReviewData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


