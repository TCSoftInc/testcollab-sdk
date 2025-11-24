
# TestCasePayload


## Properties

Name | Type
------------ | -------------
`title` | string
`suite` | number
`project` | number
`issueKey` | string
`im` | string
`issueId` | string
`instanceId` | string
`description` | string
`steps` | [Array&lt;TestCaseStepsPayload&gt;](TestCaseStepsPayload.md)
`priority` | number
`tags` | Array&lt;number&gt;
`attachments` | Array&lt;string&gt;
`customFields` | [Array&lt;CustomFieldInputPayload&gt;](CustomFieldInputPayload.md)
`requirements` | Array&lt;number&gt;
`posterComment` | string
`reviewer` | number
`reviewStatus` | number
`autoInfo` | string

## Example

```typescript
import type { TestCasePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "title": Test case 1,
  "suite": 1,
  "project": 1,
  "issueKey": PD-1,
  "im": JIRA,
  "issueId": null,
  "instanceId": null,
  "description": This is <b>my</b> test case,
  "steps": null,
  "priority": 1,
  "tags": [1,2,4],
  "attachments": null,
  "customFields": null,
  "requirements": [1,2,4],
  "posterComment": null,
  "reviewer": null,
  "reviewStatus": null,
  "autoInfo": null,
} satisfies TestCasePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCasePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


