
# ProjectSecretRevealResult


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`value` | string

## Example

```typescript
import type { ProjectSecretRevealResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": LOGIN_PASSWORD,
  "value": my_secret_value,
} satisfies ProjectSecretRevealResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectSecretRevealResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


