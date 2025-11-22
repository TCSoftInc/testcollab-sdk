
# RolePayload


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`permissions` | Array&lt;string&gt;
`company` | number

## Example

```typescript
import type { RolePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Manager,
  "permissions": ["testCaseAdd","testCaseEdit"],
  "company": 1,
} satisfies RolePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RolePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


