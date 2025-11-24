
# StatusUpdatePayload


## Properties

Name | Type
------------ | -------------
`name` | string
`description` | string
`priority` | number
`isActive` | boolean
`color` | string
`ignoreResult` | boolean
`enableReportBug` | boolean

## Example

```typescript
import type { StatusUpdatePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Flaky Test,
  "description": Test that sometimes passes, sometimes fails unexpectedly,
  "priority": 5,
  "isActive": true,
  "color": #FFC107,
  "ignoreResult": true,
  "enableReportBug": true,
} satisfies StatusUpdatePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StatusUpdatePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


