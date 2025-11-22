
# TestPlanAssignmentPayloadAssignment

Only allowed in case of assignment_method = manual. Children objects - testCases and configuration are nullable based on assignment_criteria\'s value

## Properties

Name | Type
------------ | -------------
`user` | Array&lt;number&gt;
`testCases` | [TestCaseRefCollection](TestCaseRefCollection.md)
`_configuration` | Array&lt;number&gt;

## Example

```typescript
import type { TestPlanAssignmentPayloadAssignment } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "user": [1,2,3],
  "testCases": null,
  "_configuration": [1,2,3],
} satisfies TestPlanAssignmentPayloadAssignment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanAssignmentPayloadAssignment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


