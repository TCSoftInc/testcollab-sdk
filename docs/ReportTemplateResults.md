
# ReportTemplateResults

Aggregated results of a saved report

## Properties

Name | Type
------------ | -------------
`dataset` | string
`granularity` | string
`totalRows` | number
`dimensions` | [Array&lt;ReportDimension&gt;](ReportDimension.md)
`metrics` | [Array&lt;ReportMetric&gt;](ReportMetric.md)
`rows` | Array&lt;{ [key: string]: any; }&gt;

## Example

```typescript
import type { ReportTemplateResults } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "dataset": TestCase,
  "granularity": day,
  "totalRows": 128,
  "dimensions": null,
  "metrics": null,
  "rows": null,
} satisfies ReportTemplateResults

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReportTemplateResults
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


