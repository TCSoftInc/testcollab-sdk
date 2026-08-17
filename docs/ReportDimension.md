
# ReportDimension

A field the report groups by. Its `field` is the key that carries the grouped value on every row of the result.

## Properties

Name | Type
------------ | -------------
`field` | string
`label` | string

## Example

```typescript
import type { ReportDimension } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "field": last_run_status,
  "label": Last Run Status,
} satisfies ReportDimension

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReportDimension
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


