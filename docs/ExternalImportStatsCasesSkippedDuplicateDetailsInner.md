
# ExternalImportStatsCasesSkippedDuplicateDetailsInner


## Properties

Name | Type
------------ | -------------
`issueKey` | string
`title` | string
`duplicatedWithIssueKey` | string
`duplicatedWithTitle` | string

## Example

```typescript
import type { ExternalImportStatsCasesSkippedDuplicateDetailsInner } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "issueKey": XRS-53,
  "title": Company validations,
  "duplicatedWithIssueKey": XRS-41,
  "duplicatedWithTitle": Company validations,
} satisfies ExternalImportStatsCasesSkippedDuplicateDetailsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportStatsCasesSkippedDuplicateDetailsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


