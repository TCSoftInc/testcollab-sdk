
# ExportIssuesPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`exportAs` | string
`filterModel` | string
`sortModel` | string
`criteria` | string
`issues` | Array&lt;number&gt;
`fields` | Array&lt;string&gt;
`removeTags` | boolean

## Example

```typescript
import type { ExportIssuesPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": null,
  "exportAs": csv,
  "filterModel": null,
  "sortModel": null,
  "criteria": all,
  "issues": [1,2,3],
  "fields": ["external_id","title","issue_status","issue_manager"],
  "removeTags": null,
} satisfies ExportIssuesPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExportIssuesPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


