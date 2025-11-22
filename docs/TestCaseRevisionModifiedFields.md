
# TestCaseRevisionModifiedFields


## Properties

Name | Type
------------ | -------------
`copyOf` | number
`title` | string
`revertTo` | number
`fields` | Array&lt;string&gt;
`lastChanged` | [TestCaseRevisionReviewInfo](TestCaseRevisionReviewInfo.md)

## Example

```typescript
import type { TestCaseRevisionModifiedFields } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "copyOf": 1,
  "title": Test Case 1,
  "revertTo": 2,
  "fields": null,
  "lastChanged": null,
} satisfies TestCaseRevisionModifiedFields

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseRevisionModifiedFields
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


