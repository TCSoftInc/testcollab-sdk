
# ExternalImportSourceProject


## Properties

Name | Type
------------ | -------------
`key` | string
`name` | string
`counts` | [ExternalImportSourceProjectCounts](ExternalImportSourceProjectCounts.md)
`alreadyImported` | boolean
`lastImportId` | number
`lastImportedAt` | string

## Example

```typescript
import type { ExternalImportSourceProject } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "key": ABC,
  "name": Acme Backend,
  "counts": null,
  "alreadyImported": false,
  "lastImportId": 17,
  "lastImportedAt": 2026-04-08T12:00:00.000Z,
} satisfies ExternalImportSourceProject

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportSourceProject
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


