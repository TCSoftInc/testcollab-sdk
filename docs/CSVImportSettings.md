
# CSVImportSettings


## Properties

Name | Type
------------ | -------------
`csvFile` | number
`delimiter` | string
`recordType` | string
`hasHeader` | boolean
`selectedSuite` | number
`enableSuiteMapping` | boolean
`columnIndex` | boolean

## Example

```typescript
import type { CSVImportSettings } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "csvFile": null,
  "delimiter": ,,
  "recordType": one_per_row,
  "hasHeader": true,
  "selectedSuite": 1,
  "enableSuiteMapping": null,
  "columnIndex": true,
} satisfies CSVImportSettings

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CSVImportSettings
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


