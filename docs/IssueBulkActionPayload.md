
# IssueBulkActionPayload


## Properties

Name | Type
------------ | -------------
`actionType` | string
`project` | number
`issueIds` | Array&lt;number&gt;
`customFields` | [Array&lt;CustomFieldInputPayload&gt;](CustomFieldInputPayload.md)

## Example

```typescript
import type { IssueBulkActionPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "actionType": null,
  "project": 1,
  "issueIds": null,
  "customFields": null,
} satisfies IssueBulkActionPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as IssueBulkActionPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


