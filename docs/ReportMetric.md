
# ReportMetric

A value the report aggregates. Its `label` is the key that carries the computed number on every row of the result.

## Properties

Name | Type
------------ | -------------
`op` | string
`field` | string
`label` | string

## Example

```typescript
import type { ReportMetric } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "op": count,
  "field": id,
  "label": Count,
} satisfies ReportMetric

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReportMetric
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


