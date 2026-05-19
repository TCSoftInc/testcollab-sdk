
# DashboardWidgetLayoutItem


## Properties

Name | Type
------------ | -------------
`id` | number
`positionX` | number
`positionY` | number
`width` | number
`height` | number
`visualizationType` | string
`dashboardSection` | string

## Example

```typescript
import type { DashboardWidgetLayoutItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "positionX": 0,
  "positionY": 0,
  "width": 6,
  "height": 4,
  "visualizationType": column,
  "dashboardSection": below_static,
} satisfies DashboardWidgetLayoutItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DashboardWidgetLayoutItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


