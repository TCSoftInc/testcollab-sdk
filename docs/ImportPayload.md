
# ImportPayload


## Properties

Name | Type
------------ | -------------
`importer` | string
`project` | number
`settings` | [CSVImportSettings](CSVImportSettings.md)
`fieldMap` | [Array&lt;ImportFieldMapInner&gt;](ImportFieldMapInner.md)
`dataMap` | [Array&lt;ImportDataMapInner&gt;](ImportDataMapInner.md)

## Example

```typescript
import type { ImportPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "importer": csv,
  "project": 1,
  "settings": null,
  "fieldMap": null,
  "dataMap": null,
} satisfies ImportPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ImportPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


