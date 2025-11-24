
# IssuePayload


## Properties

Name | Type
------------ | -------------
`title` | string
`project` | number
`description` | string
`priority` | number
`status` | number
`attachments` | Array&lt;string&gt;
`customFields` | [Array&lt;CustomFieldInputPayload&gt;](CustomFieldInputPayload.md)

## Example

```typescript
import type { IssuePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "title": Issue 1,
  "project": 1,
  "description": null,
  "priority": null,
  "status": null,
  "attachments": null,
  "customFields": null,
} satisfies IssuePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as IssuePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


