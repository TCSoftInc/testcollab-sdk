
# ExternalImportStats

Running counts emitted by the import runner

## Properties

Name | Type
------------ | -------------
`suitesCreated` | number
`casesCreated` | number
`casesSkippedDuplicate` | number
`casesSkippedDuplicateKeys` | Array&lt;string&gt;
`casesSkippedDuplicateDetails` | [Array&lt;ExternalImportStatsCasesSkippedDuplicateDetailsInner&gt;](ExternalImportStatsCasesSkippedDuplicateDetailsInner.md)
`casesSkippedPreviouslyImported` | number
`testSetsCreated` | number
`testPlansCreated` | number
`manualCount` | number
`cucumberCount` | number
`genericCount` | number
`failed` | [Array&lt;ExternalImportFailedItem&gt;](ExternalImportFailedItem.md)

## Example

```typescript
import type { ExternalImportStats } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "suitesCreated": 89,
  "casesCreated": 412,
  "casesSkippedDuplicate": 18,
  "casesSkippedDuplicateKeys": ["XRS-12","XRS-18","XRS-29"],
  "casesSkippedDuplicateDetails": null,
  "casesSkippedPreviouslyImported": 24,
  "testSetsCreated": 0,
  "testPlansCreated": 0,
  "manualCount": 367,
  "cucumberCount": 38,
  "genericCount": 7,
  "failed": null,
} satisfies ExternalImportStats

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportStats
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


