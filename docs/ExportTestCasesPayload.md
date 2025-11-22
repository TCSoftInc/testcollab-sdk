
# ExportTestCasesPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`exportAs` | string
`filterModel` | string
`sortModel` | string
`criteria` | string
`testCases` | Array&lt;number&gt;
`fields` | Array&lt;string&gt;
`testPlan` | number
`configs` | Array&lt;number&gt;
`run` | number
`removeTags` | boolean

## Example

```typescript
import type { ExportTestCasesPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "project": null,
  "exportAs": csv,
  "filterModel": null,
  "sortModel": null,
  "criteria": all,
  "testCases": [1,2,3],
  "fields": ["title","priority","suite"],
  "testPlan": null,
  "configs": [1,2,3],
  "run": null,
  "removeTags": null,
} satisfies ExportTestCasesPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExportTestCasesPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


