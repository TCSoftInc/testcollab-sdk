
# ExportDefectsPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`exportAs` | string
`filterModel` | string
`sortModel` | string
`criteria` | string
`defects` | Array&lt;number&gt;
`fields` | Array&lt;string&gt;
`removeTags` | boolean
`release` | number

## Example

```typescript
import type { ExportDefectsPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": null,
  "exportAs": csv,
  "filterModel": null,
  "sortModel": null,
  "criteria": all,
  "defects": [1,2,3],
  "fields": ["external_id","title","defect_status","issue_manager"],
  "removeTags": null,
  "release": null,
} satisfies ExportDefectsPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExportDefectsPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


