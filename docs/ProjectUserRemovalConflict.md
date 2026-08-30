
# ProjectUserRemovalConflict

Returned by DELETE /projectusers/{id} when the member still holds actionable assignments. Resolve them with POST /projectusers/{id}/remove.

## Properties

Name | Type
------------ | -------------
`status` | boolean
`code` | string
`message` | string
`impact` | [ProjectUserRemovalImpact](ProjectUserRemovalImpact.md)

## Example

```typescript
import type { ProjectUserRemovalConflict } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": false,
  "code": ASSIGNMENT_RESOLUTION_REQUIRED,
  "message": This project member has assignments that must be resolved first.,
  "impact": null,
} satisfies ProjectUserRemovalConflict

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectUserRemovalConflict
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


