
# ExportRequirementsPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`exportAs` | string
`filterModel` | string
`sortModel` | string
`criteria` | string
`requirements` | Array&lt;number&gt;
`fields` | Array&lt;string&gt;
`removeTags` | boolean
`hasLinkedTestCases` | boolean

## Example

```typescript
import type { ExportRequirementsPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": null,
  "exportAs": csv,
  "filterModel": null,
  "sortModel": null,
  "criteria": all,
  "requirements": [1,2,3],
  "fields": ["title","requirement_key","requirement_folder"],
  "removeTags": null,
  "hasLinkedTestCases": null,
} satisfies ExportRequirementsPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExportRequirementsPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


