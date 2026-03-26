
# DashboardWidgetPayload


## Properties

Name | Type
------------ | -------------
`reportTemplate` | number
`project` | number
`sortOrder` | number

## Example

```typescript
import type { DashboardWidgetPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "reportTemplate": 10,
  "project": 1,
  "sortOrder": 0,
} satisfies DashboardWidgetPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DashboardWidgetPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


