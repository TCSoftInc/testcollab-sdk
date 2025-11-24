
# LoginMethod


## Properties

Name | Type
------------ | -------------
`method` | string
`isAdmin` | boolean
`allowed` | Array&lt;string&gt;
`methodInfo` | string

## Example

```typescript
import type { LoginMethod } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "method": local,
  "isAdmin": false,
  "allowed": ["okta","local"],
  "methodInfo": null,
} satisfies LoginMethod

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LoginMethod
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


