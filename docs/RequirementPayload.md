
# RequirementPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`requirementManager` | string
`title` | string
`externalId` | string
`project` | number
`requirementData` | string
`description` | string
`requirementFolder` | number
`customFields` | [Array&lt;CustomFieldInputPayload&gt;](CustomFieldInputPayload.md)
`attachments` | Array&lt;string&gt;
`testcases` | Array&lt;number&gt;

## Example

```typescript
import type { RequirementPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 2,
  "requirementManager": null,
  "title": sample test,
  "externalId": null,
  "project": 1,
  "requirementData": null,
  "description": null,
  "requirementFolder": 1,
  "customFields": null,
  "attachments": null,
  "testcases": null,
} satisfies RequirementPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RequirementPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


