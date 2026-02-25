
# ReleaseReadinessDefects

Defects linked to test plans in this release, with open count and severity breakdown. 

## Properties

Name | Type
------------ | -------------
`total` | number
`totalOpen` | number
`bySeverity` | [Array&lt;ReleaseReadinessDefectSeverity&gt;](ReleaseReadinessDefectSeverity.md)

## Example

```typescript
import type { ReleaseReadinessDefects } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "total": 35,
  "totalOpen": 20,
  "bySeverity": null,
} satisfies ReleaseReadinessDefects

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessDefects
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


