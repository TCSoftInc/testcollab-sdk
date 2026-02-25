
# ReleaseReadinessEvidence

Metrics about test evidence (attachments) on executed test cases, particularly for failed executions. 

## Properties

Name | Type
------------ | -------------
`totalFailed` | number
`failedWithAttachments` | number
`evidenceCoverage` | number

## Example

```typescript
import type { ReleaseReadinessEvidence } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "totalFailed": 32,
  "failedWithAttachments": 28,
  "evidenceCoverage": 87.5,
} satisfies ReleaseReadinessEvidence

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessEvidence
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


