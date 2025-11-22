
# TestCaseQuickUpdate


## Properties

Name | Type
------------ | -------------
`id` | number
`suite` | number
`priority` | number
`tags` | Array&lt;number&gt;
`overwriteTags` | boolean
`customFields` | [Array&lt;CustomFieldInputPayload&gt;](CustomFieldInputPayload.md)
`requirements` | Array&lt;number&gt;
`overwriteRequirements` | boolean

## Example

```typescript
import type { TestCaseQuickUpdate } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "suite": 1,
  "priority": 1,
  "tags": [1,2,4],
  "overwriteTags": false,
  "customFields": null,
  "requirements": [1,2,4],
  "overwriteRequirements": false,
} satisfies TestCaseQuickUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseQuickUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


