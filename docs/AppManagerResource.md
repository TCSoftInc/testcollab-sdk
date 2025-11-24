
# AppManagerResource


## Properties

Name | Type
------------ | -------------
`company` | number
`name` | string
`resourceList` | [Array&lt;AppManagerResourceItem&gt;](AppManagerResourceItem.md)
`resourceInfo` | string

## Example

```typescript
import type { AppManagerResource } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "company": 1,
  "name": null,
  "resourceList": null,
  "resourceInfo": null,
} satisfies AppManagerResource

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AppManagerResource
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


