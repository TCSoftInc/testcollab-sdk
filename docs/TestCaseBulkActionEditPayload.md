
# TestCaseBulkActionEditPayload


## Properties

Name | Type
------------ | -------------
`overwriteTags` | boolean
`suite` | number
`priority` | number
`tags` | Array&lt;number&gt;
`customFields` | [Array&lt;CustomFieldInputPayload&gt;](CustomFieldInputPayload.md)
`requirements` | Array&lt;number&gt;
`overwriteRequirements` | boolean

## Example

```typescript
import type { TestCaseBulkActionEditPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "overwriteTags": false,
  "suite": 1,
  "priority": 1,
  "tags": [1,2,4],
  "customFields": null,
  "requirements": [1,2,4],
  "overwriteRequirements": false,
} satisfies TestCaseBulkActionEditPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseBulkActionEditPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


