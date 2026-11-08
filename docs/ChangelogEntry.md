
# ChangelogEntry


## Properties

Name | Type
------------ | -------------
`id` | string
`date` | string
`category` | string
`title` | string
`summary` | string

## Example

```typescript
import type { ChangelogEntry } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 2026-11-06-risk-based-testing-on-elite,
  "date": 2026-11-06,
  "category": improvement,
  "title": Risk-Based Testing is now included in Elite,
  "summary": Elite plans now include Risk-Based Testing.,
} satisfies ChangelogEntry

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ChangelogEntry
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


