
# ProjectsettingPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`settingType` | string
`settings` | [Array&lt;Projectsetting&gt;](Projectsetting.md)

## Example

```typescript
import type { ProjectsettingPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 1,
  "settingType": general,
  "settings": null,
} satisfies ProjectsettingPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectsettingPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


