
# RequirementProfilePayload


## Properties

Name | Type
------------ | -------------
`name` | string
`requirementManager` | string
`_configuration` | string

## Example

```typescript
import type { RequirementProfilePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Main bug tracker,
  "requirementManager": JIRA,
  "_configuration": {},
} satisfies RequirementProfilePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RequirementProfilePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


