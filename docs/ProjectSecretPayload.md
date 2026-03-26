
# ProjectSecretPayload


## Properties

Name | Type
------------ | -------------
`name` | string
`value` | string
`description` | string
`project` | number

## Example

```typescript
import type { ProjectSecretPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": LOGIN_PASSWORD,
  "value": my_secret_value,
  "description": Login password for staging environment,
  "project": 1,
} satisfies ProjectSecretPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectSecretPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


