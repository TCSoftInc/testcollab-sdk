
# Projectsetting


## Properties

Name | Type
------------ | -------------
`name` | string
`value` | string
`label` | string
`project` | [ProjectMini](ProjectMini.md)

## Example

```typescript
import type { Projectsetting } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": dateFormat,
  "value": m-d-yy,
  "label": Date format,
  "project": null,
} satisfies Projectsetting

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Projectsetting
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


