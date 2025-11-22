
# UserPreference


## Properties

Name | Type
------------ | -------------
`lastAccessedProjects` | [Array&lt;LastAccessedProject&gt;](LastAccessedProject.md)
`notification` | [Array&lt;PreferencePayload&gt;](PreferencePayload.md)

## Example

```typescript
import type { UserPreference } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "lastAccessedProjects": null,
  "notification": null,
} satisfies UserPreference

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UserPreference
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


