
# TestCaseQuickUpdatePayload


## Properties

Name | Type
------------ | -------------
`testcases` | Array&lt;number&gt;
`overwriteTags` | boolean
`suite` | number
`priority` | number
`tags` | Array&lt;number&gt;
`customFields` | [Array&lt;CustomFieldInputPayload&gt;](CustomFieldInputPayload.md)
`requirements` | Array&lt;number&gt;
`overwriteRequirements` | boolean

## Example

```typescript
import type { TestCaseQuickUpdatePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "testcases": [1,2,4],
  "overwriteTags": false,
  "suite": 1,
  "priority": 1,
  "tags": [1,2,4],
  "customFields": null,
  "requirements": [1,2,4],
  "overwriteRequirements": false,
} satisfies TestCaseQuickUpdatePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseQuickUpdatePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


