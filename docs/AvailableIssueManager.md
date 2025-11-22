
# AvailableIssueManager


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`logo` | string
`configFields` | [Array&lt;IssueManagerConfigField&gt;](IssueManagerConfigField.md)

## Example

```typescript
import type { AvailableIssueManager } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": JIRA,
  "logo": https://i.pravatar.cc/100,
  "configFields": [{"id":1,"name":"url","label":"JIRA URL","type":"url","default_value":null,"is_required":true,"extra":{}},{"id":2,"name":"api_token","label":"API Token","type":"text","default_value":null,"is_required":true,"extra":{}}],
} satisfies AvailableIssueManager

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AvailableIssueManager
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


