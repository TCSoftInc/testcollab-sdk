
# CopyToOtherProjectPayload


## Properties

Name | Type
------------ | -------------
`ids` | Array&lt;number&gt;
`project` | number
`targetProject` | number
`targetSuite` | number
`reviewer` | number
`doNotCopySuites` | boolean

## Example

```typescript
import type { CopyToOtherProjectPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "ids": [1,2],
  "project": 3,
  "targetProject": null,
  "targetSuite": null,
  "reviewer": null,
  "doNotCopySuites": null,
} satisfies CopyToOtherProjectPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CopyToOtherProjectPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


