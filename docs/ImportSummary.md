
# ImportSummary


## Properties

Name | Type
------------ | -------------
`importCount` | number
`failedCount` | number
`errorLog` | string

## Example

```typescript
import type { ImportSummary } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "importCount": 230,
  "failedCount": 4,
  "errorLog": Failed to import xyz because of qwert\n Failed to import kfkf because of rtrtt
,
} satisfies ImportSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ImportSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


